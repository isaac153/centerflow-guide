# 상담 환경 설정

&#x20;**서비스 관리 > 상담 애플리케이션 > 상담 환경 설정** 메뉴에서는 상담 애플리케이션에 적용할 기본 상담 정책을 설정할 수 있습니다.&#x20;

{% hint style="info" %}
**안내**

* 회원 상태가 ‘시작 요청 전’인 경우에 한하여 설정 가능합니다.
* 서비스 시작 요청이 완료된 시점부터는 설정된 내용을 콘솔에서 수정할 수 없습니다.
* 설정 내용 수정을 희망하시면, [서비스 지원 문의](https://centerflow.kakaocloud.com/support)를 접수해 주세요.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (130).png" alt=""><figcaption><p>상담 환경 설정</p></figcaption></figure>

<table><thead><tr><th width="213">구분</th><th>설명</th></tr></thead><tbody><tr><td>⓵ 테넌트명</td><td>상담앱 ID에 사용될 상담앱의 고유 식별 문자 설정</td></tr><tr><td>⓶ 고객센터 대표번호</td><td>고객센터에 전화를 걸 때 사용하는 수신용 번호 설정<br>- 번호 개통 전일 경우, 생략 가능</td></tr><tr><td>⓷ 고객센터 발신번호</td><td>상담사가 고객에게 전화를 걸 때 사용하는 발신용 번호 설정 <br>- 번호 개통 전일 경우, 생략 가능</td></tr><tr><td>⓸ 상담 업무 유형 <br>   (상담 스킬)</td><td>상담사별로 상담 업무를 배정할 때 사용하는 상담사의 담당 업무 유형 설정</td></tr><tr><td>⓹ 상담 결과 유형</td><td>상담 결과를 분류할 때 사용되는 상담 결과 유형 설정</td></tr><tr><td>⓺ 상담사 근무 정책</td><td>상담 업무 시간 설정 <br>- 휴게시간과 비근무시간에는 상담사 연결 불가하여 IVR 안내 메시지 송출</td></tr><tr><td>⓻ 실물 전화기 신청</td><td>실물 전화기 신청 여부 선택</td></tr></tbody></table>

## 상담 업무 유형 (상담 스킬) <a href="#skill" id="skill"></a>

### 상담 업무 유형 등록

상담 업무 유형(상담 스킬) ‘등록하기’를 클릭하여 상담 업무의 유형을 등록할 수 있습니다. +, - 버튼으로 업무 유형 입력란 추가/삭제가 가능합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/%EC%83%81%EB%8B%B4%20%EC%97%85%EB%AC%B4%20%EC%9C%A0%ED%98%95%20%EB%93%B1%EB%A1%9D.png" alt=""><figcaption><p>상담 업무 유형 등록</p></figcaption></figure>

### 상담 업무 배정 <a href="#type" id="type"></a>

구독 신청 시 입력한 상담사 및 상담+관리자 수량만큼 행이 노출됩니다. 각 권한에 따라 상담사 이름(선택값)을 입력하고, ‘상담 업무 유형 등록’에서 입력한 담당 상담 업무를 선택합니다. 등록된 상담 업무는 모두 상담사에게 배정되어야 합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/%EC%83%81%EB%8B%B4%20%EC%97%85%EB%AC%B4%20%EB%B0%B0%EC%A0%95.png" alt=""><figcaption><p>상담 업무 배정</p></figcaption></figure>



### 상담사 근무 정책 <a href="#policy" id="policy"></a>

상담사의 상담 업무시간을 설정합니다. 근무 요일, 근무 시간, 휴게시간을 이미 등록되어 있는 템플릿 중에 선택할 수 있으며, 원하는 업무 시간 템플릿이 없을 경우 ‘직접 입력’을 클릭해 원하는 근무 요일, 시간, 휴게시간 템플릿을 등록할 수 있습니다. 근무할 요일을 선택하고, 시간을 입력한 뒤 +를 누르면 근무일정 템플릿이 생성됩니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/%EC%83%81%EB%8B%B4%EC%82%AC%20%EA%B7%BC%EB%AC%B4%20%EC%A0%95%EC%B1%85.png" alt=""><figcaption><p>상담사 근무 정책</p></figcaption></figure>



