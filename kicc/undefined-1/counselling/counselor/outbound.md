# 콜백 (아웃바운드 상담)

고객이 상담 요청을 위해 발신을 시도할 경우 IVR(ARS)장치에 먼저 착신이 되고 ARS메뉴에서 상담사 연결을 시도하거나 상담사가 전화를 받지 못할 경우, 전화음성봇 또는 IVR을 통해 콜백 요청을 등록할 수 있습니다.&#x20;

스마트접수를 통해 상담사 연결을 시도한 경우에도 상담사가 부재하면 콜백 등록이 가능합니다.

## 콜백 Flow <a href="#call-back-flow" id="call-back-flow"></a>

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%BD%9C%EB%B0%B1%20flow.png" alt=""><figcaption><p>콜백 flow</p></figcaption></figure>

## 콜백 조회 <a href="#inquiry-call-back" id="inquiry-call-back"></a>

IVR과 AI 상담봇에서 등록한 콜백 리스트(테넌트별)를 조회합니다.

* 관리자 권한의 상담사가 콜백 분배를 해야 할 목록 조회

<table><thead><tr><th width="158">필드명</th><th>설명</th></tr></thead><tbody><tr><td>등록일자</td><td>콜백 등록 일자</td></tr><tr><td>상담사ID</td><td>상담사에게 콜백이 할당된 경우 상담사ID로 표기됨<br>상담사 ID가 null인 경우 콜백 미할당된 목록</td></tr><tr><td>고객 번호</td><td>콜백 등록을 요청한 발신측 전화번호</td></tr><tr><td>콜백 번호</td><td>콜백 받을 전화번호 ( 고객 번호와 동일 또는 다르게 설정됨 )</td></tr><tr><td>발신 일자</td><td>콜백 발신을 시도한 일자</td></tr><tr><td>처리 상태</td><td>미처리 : 상담사에게 콜백 분배가 되지 않거나, 상담사에게 분배는 되었으나 콜백 호를 시도하지 않은 경우<br>처리완료 : 상담사가 콜백 발신을 시도한 경우</td></tr><tr><td>콜백 유형</td><td>일반 콜백 : IVR 시나리오를 통해 콜백을 등록한 경우<br>스마트콜백 : AI 상담봇을 통해 콜백을 등록한 경우<br>스마트접수 : 스마트접수를 설정한 상담봇의 세부문의를 통해 콜백을 등록한 경우</td></tr><tr><td>강제처리 완료</td><td>등록된 콜백 리스트에 대해서 강제 처리<br>- 동일한 사용자가 다수의 콜백을 남긴 경우 상담사가 콜백을 한번만 해도 해당 사용자의 콜백 목록을 일괄로 삭제하도록 동작<br>- 콜백 생성과정에서 고객번호, 콜백번호가 비정상적으로 등록이 된 경우에 콜백 발신을 하지 않고 강체 처리 완료를 할 수 있음</td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

## 콜백 분배 <a href="#distribute" id="distribute"></a>

상담사별로 할당된 콜백에 대해서 일괄회수, 개별 회수 기능을 제공합니다. 등록된 콜백 리스트를 각 부서(테넌트, 그룹, 파트,상담사)내 상담사로 분배합니다.

#### **분배 대상 조회**

| 필드명   | 설명                                                           |
| ----- | ------------------------------------------------------------ |
| 조회 기간 | 콜백이 등록된 시간                                                   |
| 테넌트   | 콜백을 분배할 상담사 범위를 지정                                           |
| 그룹    |                                                              |
| 파트    |                                                              |
| 분배    | <p>상담사 <br>파트 매니저 <br>그룹 메니저 <br>테넌트 메니저 </p>                |
| 콜백 유형 | <p>IVR 콜백 = IVR(ARS)장치에서 추가한 콜백<br>AI 콜백 = AI콜봇에서 추가한 콜백</p> |

#### **분배 정책 (일괄 분배)**

상담사별로 일괄 콜백을 분배하거나 특정 상담사별로 개별 분배를 설정할 수 있습니다. 일괄 분배 시 총 대상 건수가 분배할 상담사보다 많은 경우에 한해서 설정이 가능합니다.

<table><thead><tr><th width="166">필드명</th><th>설명</th></tr></thead><tbody><tr><td>총 대상 건</td><td>분배되지 않은 콜백의 수</td></tr><tr><td>총 분배량</td><td>분배된 콜백의 수</td></tr><tr><td>총 사용량</td><td>분배된 콜백 중 처리된 수</td></tr><tr><td>총 미사용량</td><td>분배된 콜백 중 미처리된 수</td></tr><tr><td>1인당 분배</td><td>상담사별로 균등하게 콜백을 분배하기 위한 수</td></tr><tr><td>1인당 회수</td><td>상담사별로 분배된 콜백을 회수하기 위한 수</td></tr><tr><td>총 미분배 건수</td><td>상담사별로 분배되지 않은 콜백 수</td></tr></tbody></table>

* 총 대상건수 2건에 대해서 상담사가 3명일 경우 균등 분배 불가
* 총 대상건수 2건에 대해서 상담사가 2명인 경우 상담사별로 1건의 콜백이 분배됨
* 총 대상건수 3건에 대해서 상담사가 2명인 경우 상담사별로 1건의 콜백이 분배되고 나머지 1건은 미 분배로 처리됨

#### **분배 정책 (개별 분배)**

상담사별로 콜백을 분배할 수 있습니다. 상담사를 선택 후 분배(입력)칸에 분배할 수를 입력하고 “분배실행”을 클릭하면 적용됩니다. 특정 콜백 목록을 특정 상담사에게 지정해서 분배하는 기능은 제공하지 않습니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%BD%9C%EB%B0%B1%20%EB%B6%84%EB%B0%B0.png" alt=""><figcaption><p>콜백 분배</p></figcaption></figure>

#### **분배 결과 조회**

상담사별 콜백 분배된 현황을 확인하거나 해당 상담사에게 콜백을 개별 할당할 수 있습니다.

| 필드명     | 설명                                      |
| ------- | --------------------------------------- |
| 팀명      | 상담사가 소속된 팀명                             |
| 이름      | 상담사                                     |
| 분배 건수   | 관리자가 해당 상담사에게 콜백을 분배한 건수                |
| 사용 건수   | 상담사가 분배된 콜백 목록을 이용하여 콜백 발신을 시도한 건수      |
| 미사용 현황  | 상담사로 콜백 분배는 되었으나 상담사가 콜백 발신을 시도하지 않은 건수 |
| 분배 (입력) | 상담사별 콜백 개별 분배                           |
| 회수 (입력) | 상담사별로 분배된 콜백을 개별 회수                     |

## 콜백 회수 <a href="#retrieve" id="retrieve"></a>

상담사별로 할당된 콜백에 대해서 일괄회수, 개별 회수 기능을 제공합니다.

#### **회수 정책 (일괄 회수)**

상담사별로 할당된 콜백에 대해서 일괄로 회수를 진행할 수 있습니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%BD%9C%EB%B0%B1%20%EC%9D%BC%EA%B4%84%20%ED%9A%8C%EC%88%98.png" alt=""><figcaption><p>콜백 일괄 회수</p></figcaption></figure>

#### **분배 정책 (개별 회수)**

특정 상담사에게 할당된 콜백에 대한 회수를 진행할 수 있습니다. 상담사를 선택 후 분배(입력)칸에 분배할 수를 입력하고 “회수실행”을 클릭하면 적용됩니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%BD%9C%EB%B0%B1%20%EA%B0%9C%EB%B3%84%20%ED%9A%8C%EC%88%98.png" alt=""><figcaption><p>콜백 개별 회수</p></figcaption></figure>

## 콜백 발신 <a href="#callback-details" id="callback-details"></a>

상담사별로 할당된 콜백 목록은  콜상담 메뉴의 “상담리스트 탭 – 콜백”에 자동으로 표시됩니다.

상담사는 해당 콜백 목록을 더블클릭하면 전화번호 키패드 입력창에 발신할 전화번호가 표시되고 해당 전화번호에 대해서 상담 고객으로등록이 된 경우 해당 고객정보가 표시됩니다. 상담 고객으로 등록되지 않은 경우 콜백 상담을 실시하고 신규 고객으로 생성합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%BD%9C%EB%B0%B1%20%EB%B0%9C%EC%8B%A0.png" alt=""><figcaption><p>콜백 발신</p></figcaption></figure>

## 콜백 삭제 <a href="#delete-callback" id="delete-callback"></a>

콜백 목록을 선택하여 아웃바운드 상담전화를 시도하고 상담 결과를 저장해야만 상담사별로 분배된 콜백 목록이 삭제됩니다.

콜백 목록에 동일한 고객이 다수 등록된 경우  콜백 발신을 1회 진행한 경우 일괄 삭제 처리됩니다.  비정상적인 콜백 번호인 경우 강제처리 완료를 통해서 콜백 목록에서 삭제합니다. 분배된 전체 콜백 목록에 대해서 아웃바운드 콜백 상담을 완료한 경우  콜백탭에는 count가 0으로 표시되고, 콜백 리스트에 콜백 처리 결과를 확인할 수 있습니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%BD%9C%EB%B0%B1%20%EC%82%AD%EC%A0%9C.png" alt=""><figcaption><p>콜백 삭제</p></figcaption></figure>
