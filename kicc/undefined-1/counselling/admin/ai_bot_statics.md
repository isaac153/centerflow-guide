# AI 상담봇 통계

## AI 상담봇 통계 <a href="#ai-counselor-stats" id="ai-counselor-stats"></a>

AI 상담봇과 관련된 통계를 확인할 수 있습니다.

### 날짜

날짜를 선택하여 선택한 날짜에 대한 통계를 확인할 수 있습니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%82%A0%EC%A7%9C.png" alt=""><figcaption><p>날짜</p></figcaption></figure>

<table><thead><tr><th width="135">카테고리</th><th>설명</th></tr></thead><tbody><tr><td>오늘</td><td>0시부터(운영 시간의 경우 근무 시작 시간부터) 통계를 확인하는 시점까지의 통계를 확인할 수 있음</td></tr><tr><td>어제</td><td>확인하는 시점 기준 전날의 통계를 확인할 수 있음</td></tr><tr><td>7일</td><td>확인하는 시점의 당일을 포함, 이전 7일 동안의 통계를 확인할 수 있음</td></tr><tr><td>30일</td><td>확인하는 시점의 당일을 포함, 이전 30일 동안의 통계를 확인할 수 있음</td></tr><tr><td>직접 입력</td><td>통계 확인이 필요한 날짜를 직접 지정 가능하며, 최대 3개월까지 조회할 수 있음</td></tr></tbody></table>

#### 다운로드

보고 있는 날짜에 대한 통계 데이터를 다운로드할 수 있는 기능으로 \[다운로드] 버튼을 클릭하면 아래와 같은 형태의 xlsx 파일이 다운로드됩니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%ED%86%B5%EA%B3%84%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C.png" alt=""><figcaption><p>통계 데이터 다운로드</p></figcaption></figure>

### 응대실적

AI 상담봇으로 인입된 이후의 플로우에서 AI 상담봇이 응대한 케이스별 실적을 보여줍니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%9D%91%EB%8C%80%20%EC%8B%A4%EC%A0%81.png" alt=""><figcaption><p>응대 실적</p></figcaption></figure>

**전체 시간 보기**

근무 외 시간을 포함하여, AI 상담봇이 응대하는 전체 시간에 대한 통계를 제공합니다.

**운영 시간 보기**

근무 시간에 대한 통계만을 제공합니다. 상담사 전환 후 완료 케이스의 경우 근무시간 내에만 발생하므로 전체 시간 보기에 비해 더 많은 비중을 차지할 수 있습니다.

**총 인입 기준**

누적 그래프로 노출하여 총 인입 수 중 각 케이스가 차지하는 비중을 파악하기에 용이합니다.

**개별 인입 기준**

개별 그래프로 노출하여 각 케이스의 개별 수치를 파악하기에 용이합니다.

<table><thead><tr><th width="184">범주</th><th width="456.3333333333333">설명</th><th> </th></tr></thead><tbody><tr><td>AI 상담봇 완료</td><td>상담사 전환 없이 숏헤드 인텐트 응대만으로 종료된 콜 수</td><td></td></tr><tr><td>스마트 콜백 접수</td><td>스마트 콜백이 접수된 수(IVR 콜백 포함)</td><td></td></tr><tr><td>상담사 전환 후 완료</td><td>AI 상담봇과 통화 중 상담사로 전환하여 통화 종료된 수</td><td>대시보드</td></tr><tr><td>비정상 종료</td><td>정상적으로 통화가 종료되기 전, 고객이 먼저 통화 종료한 수</td><td></td></tr></tbody></table>

### 점유율 및 완료율

#### 점유율

신청한 봇 채널이 얼마나 이용되고 있는지 보여주는 지표입니다. 비율이 낮을 수록 봇이 적게, 비율이 높을 수록 봇이 많이 사용되고 있는 것으로, 항상 높은 비율을 유지한다면 봇 채널 수를 늘리는 것이 좋습니다.

#### 완료율

전체 콜 인입 중 AI 상담봇만으로 상담을 완료한 비율입니다. 완료율이 높다면 AI 상담봇의 응대가 효율적으로 이루어지고 있다는 것을 보여줍니다.

### 인텐트별 실적

인텐트란 동일한 의도를 가진 발화들의 묶음으로, 콘솔에서 설정한 [고객 문의 유형](https://kakaoenterprise.gitbook.io/centerflow/guide/console/ai_config/response#inquiry-type)을 말합니다. 인텐트별 실적에서는 AI 상담봇이 응대한 인텐트에 대한 실적을 확인할 수 있습니다.

#### 상위 5개 인텐트

전체 인텐트 중 선택한 기간동안 가장 많이 들어온 상위 5개 인텐트에 대한 값을 보여줍니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%9D%B8%ED%85%90%ED%8A%B8%EB%B3%84%20%EC%8B%A4%EC%A0%81.png" alt=""><figcaption><p>인텐트별 실적</p></figcaption></figure>

#### 전체 인텐트

선택한 기간의 전체 인텐트에 대한 실적을 보여줍니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%A0%84%EC%B2%B4%20%EC%9D%B8%ED%85%90%ED%8A%B8.png" alt=""><figcaption><p>전체 인텐트</p></figcaption></figure>

### 평균 통화 시간

AI 상담봇이 고객을 응대하는 시간의 평균을 보여줍니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%ED%8F%89%EA%B7%A0%20%ED%86%B5%ED%99%94%20%EC%8B%9C%EA%B0%84.png" alt=""><figcaption><p>평균 통화 시간</p></figcaption></figure>

### 미지원 문의 고객 발화 분석

미지원 문의 고객 발화는 고객이 설정한 인텐트(문의 유형)에서 벗어나 AI 상담봇이 대응하지 못하는(fallback) 발화들입니다. 미지원 문의지만 많이 들어오는 유형의 발화는 [서비스 지원 문의](https://pages.kakaoenterprise.com/centerflow_support.html)를 접수하여 문의 유형을 추가하거나 [AI 답변 추천](https://guide.centerflow.kakaocloud.com/guide/console/ai_config/recommended)으로 봇 응대율을 높여주시기 바랍니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AF%B8%EC%A7%80%EC%9B%90%20%EB%AC%B8%EC%9D%98%20%EA%B3%A0%EA%B0%9D%20%EB%B0%9C%ED%99%94%20%EB%B6%84%EC%84%9D.png" alt=""><figcaption><p>미지원 문의 고객 발화 분석</p></figcaption></figure>

### 인텐트별 흐름 현황

고객이 AI 상담봇으로 전화를 걸고 통화를 종료할 때까지의 인텐트 흐름을 확인할 수 있습니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%9D%B8%ED%85%90%ED%8A%B8%EB%B3%84%20%ED%9D%90%EB%A6%84%20%ED%98%84%ED%99%A9.png" alt=""><figcaption><p>인텐트별 흐름 현황</p></figcaption></figure>
