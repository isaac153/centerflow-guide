# 매니지먼트

## 상담사 <a href="#counselor" id="counselor"></a>

### 상담사 그룹 <a href="#group" id="group"></a>

상담사 그룹을 추가/삭제/변경합니다.

* 상담사는 상담사 팀의 종속 자원이며, 상담사 팀은 상담사 그룹의 종속 자원입니다. 즉, 상담사 그룹은 상담사 자원의 최상위 모임으로 상담사를 등록하기 위해서는 반드시 등록되어야 합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%EC%82%AC%20%EA%B7%B8%EB%A3%B9.png" alt=""><figcaption><p>상담사 그룹</p></figcaption></figure>

<table><thead><tr><th width="153">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 선택</td></tr><tr><td>상담사 그룹 ID</td><td>사용하고자 하는 상담사 그룹의 ID</td></tr><tr><td>그룹명</td><td>사용하고자 하는 상담사 그룹의 이름</td></tr><tr><td>감시</td><td>상담사 그룹에 대한 감시 여부 설정 (감시 설정/감시 해제)<br>감시 설정이 활성화된 상담사 그룹에 소속된 상담사 단말에 대한 상태 모니터링이 가능</td></tr></tbody></table>

### 상담사 팀 <a href="#team" id="team"></a>

상담사 팀을 추가/삭제/변경합니다.

* 상담사는 상담사 팀의 종속 자원이며, 상담사 팀은 상담사 그룹의 종속 자원입니다. 상담사 팀은 상담사 자원의 상위 모임으로, 상담사를 등록하기 위해서는 반드시 등록되어야 합니다.

<table><thead><tr><th width="154">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>상담사 그룹이 소속될 테넌트 ID</td></tr><tr><td>그룹 ID</td><td>상담사 팀이 소속될 상담사 그룹 ID</td></tr><tr><td>팀 ID</td><td>사용하고자 하는 상담사 팀 ID</td></tr><tr><td>팀명</td><td>사용하고자 하는 상담사 팀 이름</td></tr><tr><td>감시</td><td>상담사 파트에 대한 감시 여부 설정 (감시 설정/감시 해제)<br>감시 설정이 활성화된 상담사 파트에 소속된 상담사 단말에 대한 상태 모니터링이 가능</td></tr></tbody></table>

### 상담사 <a href="#counselor" id="counselor"></a>

상담사를 추가/삭제/변경합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%EC%82%AC.png" alt=""><figcaption><p>상담사</p></figcaption></figure>

<table><thead><tr><th width="158">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>상담사 그룹이 소속될 테넌트 ID</td></tr><tr><td>그룹</td><td>상담사가 소속될 상담사 그룹ID</td></tr><tr><td>팀</td><td>상담사가 소속될 상담사 팀 ID</td></tr><tr><td>상위 상담사 ID</td><td>대표 상담사 ID</td></tr><tr><td>상담사 ID</td><td>상담사의 계정으로 사용될 ID</td></tr><tr><td>상담사</td><td>사용하고자 하는 상담사 이름</td></tr><tr><td>비밀번호</td><td>상담사ID의 비밀번호<br>- 아래 <strong>비밀번호 유의사항</strong> 참고</td></tr><tr><td>레벨</td><td>[1] 상담사<br>[2] 파트 매니저<br>[3] 그룹 매니저<br>[4] 테넌트 매니저<br>[5] 시스템 매니저<br>[6] 전체</td></tr><tr><td>권한</td><td>등록된 권한 중에 하나를 선택함</td></tr><tr><td>Blend 종류</td><td>상담사의 블랜딩 종류 선택(Inbound / Outbound / Blend)</td></tr><tr><td>업무 종류</td><td>[1] call = 콜 상담 업무용<br>[2] talk = 채팅 상담 업무용<br>[3] email =이메일 상담 업무용</td></tr><tr><td>미디어</td><td>미디어 서버</td></tr><tr><td>미디어 로그인 ID</td><td>미디어 로그인 ID</td></tr><tr><td>내선</td><td>내선 ID</td></tr><tr><td>감시</td><td>상담원의 모니터링 여부를 표시함<br>감시가 해제된 상담원은 호 분배를 받을 수 없을 뿐만 아니라 상담원 관련 호, 상태 통계도 적용되지 않음<br>※ 체크박스 체크 시: 감시 설정 / 체크 해제 시: 감시 해제</td></tr><tr><td>기본 큐</td><td>상담사가 기본적으로 분배 받을 큐 번호 선택<br>큐의 대기율(대기호수 / 수신 가능 상담원 × 100)을 이용하여 시나리오를 분배할 때에 여기에서 설정한 기본 큐의 대기호수 사용</td></tr><tr><td>접속 가능 IP</td><td>접속을 허용할 Client측 IP를 미리 등록하여 접속 여부를 제어할 수 있고 <code>*</code> 로 설정할 경우 모든 IP대역에 대해서 접속이 가능한 상태</td></tr><tr><td>이메일</td><td>상담사 이메일 주소</td></tr><tr><td>모바일</td><td>상담사 핸드폰 번호</td></tr><tr><td>팩스</td><td>상담사 팩스 번호</td></tr><tr><td>내선번호</td><td>상담사 내선번호</td></tr><tr><td>별명</td><td>상담사 별명</td></tr><tr><td>호스트명</td><td>상담사 개인 설정 도메인 또는 호스트명</td></tr><tr><td>로그인 실패 횟수</td><td>상담앱으로 로그인을 실패한 횟수가 5회가 되면 접속이 차단되며, 관리자가 로그인 실패 횟수를 0으로 초기화 하고 상담 애플리케이션의 ID와 PW를 정확하게 입력한 경우에 로그인에 성공합니다.</td></tr><tr><td>webRTC사용</td><td>상담 애플리케이션 화면에서 제공하는 통화 기능 사용 여부를 설정<br>ON = 상담 애플리케이션에서 제공하는 webRTC를 이용하여 통화할 경우 on으로 설정<br>OFF = IP-Phone을 이용하여 통화를 할 경우 off로 설정</td></tr><tr><td>Monitoring 유지시간 체크</td><td>상담 애플리케이션 화면에서 아무런 동작을 하지 않고 대기 상태만 유지될 경우 Monitoring 유지시간 경과 시 해당 세션은 강제 종료</td></tr><tr><td>콜 모니터링</td><td>‘모니터링-현황-상담사’화면에서 상담사의 통화 내용을 모니터링(감청) 할 수 있는 권한</td></tr><tr><td>비밀번호 <br>업데이트 시각</td><td>상담사의 로그인 비밀번호를 업데이트 한 시각</td></tr><tr><td>입사일</td><td>상담사 입사일</td></tr><tr><td>퇴사일</td><td>상담사 퇴사일</td></tr></tbody></table>

{% hint style="warning" %}
#### **비밀번호 유의사항**

* 비밀번호는 9-16글자로 구성되어야 합니다.
* 영문 대문자, 영문 소문자, 숫자가 각각 한 글자 이상 반드시 포함되어 있어야 합니다. (A-Z, a-z, 0-9)
* 특수문자(<mark style="color:red;">`!`</mark>`,`<mark style="color:red;">`@`</mark>`,`<mark style="color:red;">`#`</mark>`,`<mark style="color:red;">`$`</mark>`,`<mark style="color:red;">`%`</mark>`,`<mark style="color:red;">`^`</mark>`,`<mark style="color:red;">`&`</mark>`,`<mark style="color:red;">`.`</mark>`,`<mark style="color:red;">`*`</mark>`,`<mark style="color:red;">`(`</mark>`,`<mark style="color:red;">`)`</mark>`)`가 한 글자 이상 반드시 포함되어 있어야 합니다.
* 연속된 문자를 3개 이상 사용할 수 없습니다. (예: abc, 123)
* 동일한 문자를 연속으로 3개 이상 사용할 수 없습니다. (예: aaa, 111)
* 비밀번호에 ID를 포함할 수 없습니다.
{% endhint %}

생성된 상담사에 대한 스킬 부여는 상담사 목록의 제일 앞에 있는 \[add skill] 아이콘을 사용합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%EC%82%AC%20%EC%8A%A4%ED%82%AC%20%EB%B6%80%EC%97%AC.png" alt=""><figcaption><p>상담사 스킬 부여</p></figcaption></figure>

### 계정 활성화 및 비밀번호 설정 방법

* **비밀번호 5회 이상 실패시:** 상담사(agent) 로그인 시 5회 이상 비밀번호 실패할 경우 로그인을 시도할 수 없게 됩니다. 그럴 경우 admin 관리자가 상담앱 어드민에 접속 가능하여, 매니지먼트 > 상담사 > 상담사 메뉴에서 **로그인 실패 횟수를 0으로 수정**하여 저장하면 다시 로그인 시도가 가능하게 됩니다.

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

* **기존 비밀번호를 잃어버린 경우:** 상담사(agent) 계정의 비밀번호를 잃어버린 경우, 매니지먼트 > 상담사 > 상담사 메뉴의 **비밀번호**에서 해당 상담사/관리자의 비밀번호를 재설정하여 안내가 가능합니다.

<figure><img src="../../../.gitbook/assets/Group 3466028 (1).png" alt=""><figcaption></figcaption></figure>

* **장기 미사용 계정일 경우:** 상담사(agent) 계정이 장기 미사용으로 휴면 처리 된 경우, 매니지먼트 > 상담사 > 상담사 메뉴에 해당 계정 정말 맨 앞에 **'자물쇠' 버튼**이 생성됩니다. 자물쇠 버튼을 클릭하여 장기 미사용 계정을 휴면 해제할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**관리자 계정의 활성화 및 비밀번호 설정이 필요 시**

관리자(admin) 계정의 비밀번호를 5회 이상 실패하였거나, 비밀번호를 잃어버렸거나, 계정이 장기 미사용 처리되었을 경우에는 [centerflow@kakaoenterprise.com](<mailto:centerflow@kakaoenterprise.com>)로 문의해 주세요.
{% endhint %}

### 상담사 계정별 접속 IP 및 로그인 인증번호 수신 전화번호 설정

* **접속 IP  관리:** [상담사(agent) 로그인 시](../counselor/login.md) 계정정보에 설정된 IP와 동일한 IP 환경에서만 로그인이 가능합니다. 타 IP에서 접속을 시도할 경우 로그인이 불가합니다. 사전에 admin 관리자가 상담앱 어드민에 접속 가능하여, 매니지먼트 > 상담사 > 상담사 메뉴에서 **접속가능IP를 설정**해야 합니다. (접속 가능 IP를 등록하면, 로그인 시 IP 유효성 체크 기능이 즉시 적용됩니다.)

<figure><img src="../../../.gitbook/assets/접속가능ip 설정.png" alt=""><figcaption></figcaption></figure>

* **로그인 인증번호 수신 전화번호 설정:** [상담사(agent) 로그인 시](../counselor/login.md) 계정정보에 설정된 전화번호로 2차 인증을 위한 인증번호가 발송됩니다. 인증번호를 입력해야만 로그인이 가능하며 인증번호 없이는 로그인이 불가합니다. 사전에 admin 관리자가 상담앱 어드민에 접속 가능하여, 매니지먼트 > 상담사 > 상담사 메뉴에서 **모바일 항목에 상담사 전화번호를 설정**해야 합니다. (모바일 정보 입력 완료 후, 변경한 계정 가장 왼쪽의 체크박스를 체크한 뒤, '저장'을 진행해야 변경된 정보가 정상 저장됩니다.)

<figure><img src="../../../.gitbook/assets/모바일정보 셋팅.png" alt=""><figcaption></figcaption></figure>
