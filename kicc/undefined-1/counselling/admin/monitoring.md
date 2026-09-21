# 모니터링

## 모니터링 현황 <a href="#details" id="details"></a>

모니터링 자원에 대한 실시간 모니터링을 제공합니다.

### 통합 모니터링 <a href="#integrated" id="integrated"></a>

통합 모니터링은 라우트 현황(서비스 레벨, 응답율)과 상담사 상태 리스트를 한 화면에 제공합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%ED%86%B5%ED%95%A9%20%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81.png" alt=""><figcaption><p>모니터링 통합 모니터링</p></figcaption></figure>

**자원 범위**

테넌트, 그룹, 팀을 선택하여 조회할 수 있습니다. 테넌트는 1개만 선택할 수 있습니다.

**라우트 현황**

<table><thead><tr><th width="176">구분</th><th>설명</th></tr></thead><tbody><tr><td>서비스 레벨</td><td>일정한 시간 안에 응답되거나 포기된 호의 비율</td></tr><tr><td>응답율(%)</td><td>큐에 인입된 호 중 상담사에게 분배된 호의 비율<br>(응답률 = 응답 호수 / 인입 호수 * 100)</td></tr><tr><td>대기호</td><td>큐에 인입후 상담사에게 분배되기 위해 대기 중인 호<br>  - [현황 보기] 버튼 클릭 시, 대기호 리스트 확인할 수 있음</td></tr><tr><td>총 인입</td><td>큐에 인입된 총 호수</td></tr><tr><td>실 인입 호수</td><td>큐에 실 인입된 총 호수</td></tr><tr><td>상담사 분배 호수</td><td>큐에 인입 후 상담사에 분배되어 응답한 호수</td></tr><tr><td>포기호 </td><td>큐에 인입 후 상담사에게 분배되기 전 설정한 대기 시간 이내에 고객이 끊은 호수</td></tr><tr><td>넌 서비스 호수</td><td>큐에 인입 후 CTI 시스템에서 설정한 최대 대기 시간을 초과하여 끊어진 호수</td></tr><tr><td>콜백</td><td>큐에 인입 후 콜백 큐로 넘어간 호수</td></tr><tr><td>큐 전환</td><td>큐에 인입 후 다른 큐, IVRDN, 외부 등 상담원DN을 제외한 DN으로 넘어간 호수</td></tr><tr><td>실패</td><td>큐에 인입된 호 중 분배 명령이 이루어진 시점에 물리적인 이유로 인해 분배하려던 상담석 전화로 연결할 수 없어 끊어진 호수</td></tr><tr><td>그룹호 전환</td><td>그룹호 전환되어 상담원에게 분배된 호수</td></tr><tr><td>타 센터 라우팅</td><td>타 센터로 라우팅된 호수</td></tr><tr><td>타 센터 라우팅 실패</td><td>타 센터로 라우팅 됐지만 실패된 호수</td></tr><tr><td>타 센터 인입</td><td>타 센터로부터 인입된 호수</td></tr></tbody></table>

*   대기호 아래 \[현황 보기] 버튼을 클릭해 대기호 리스트를 확인할 수 있습니다.<br>

    <figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%8C%80%EA%B8%B0%ED%98%B8%20%ED%98%84%ED%99%A9%EB%B3%B4%EA%B8%B0.png" alt=""><figcaption><p>대기호 현황보기</p></figcaption></figure>

    <figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%8C%80%EA%B8%B0%ED%98%B8%20%ED%98%84%ED%99%A9.png" alt=""><figcaption><p>대기호 현황</p></figcaption></figure>

    <table><thead><tr><th width="168">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐</td><td>큐의 일련 번호</td></tr><tr><td>큐 이름</td><td>큐의 이름</td></tr><tr><td>시간대 1~20</td><td>큐에 인입된 호 중 대기시간이 1~20초 이내인 콜의 수</td></tr><tr><td>시간대 21~40</td><td>큐에 인입된 호 중 대기시간이 21~40초 이내인 콜의 수</td></tr><tr><td>시간대 41~60</td><td>큐에 인입된 호 중 대기시간이 41~60초 이내인 콜의 수</td></tr><tr><td>시간대 61~80</td><td>큐에 인입된 호 중 대기시간이 61~80초 이내인 콜의 수</td></tr><tr><td>시간대 81~300</td><td>큐에 인입된 호 중 대기시간이 81~300초 이내인 콜의 수</td></tr><tr><td>시간대 301~</td><td>큐에 인입된 호 중 대기시간이 301초 이상인 콜의 수</td></tr></tbody></table>

**상담사 상태 리스트**

상담사별 상태, 상태 사유, 유지 시간 등을 리스트 형식으로 보여줍니다.

<table><thead><tr><th width="174">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>상담사 ID</td><td>상담사 ID</td></tr><tr><td>상담사</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 그룹 ID, 상담사 그룹 이름</td></tr><tr><td>팀</td><td>상담사 팀 ID, 상담사 팀 이름</td></tr><tr><td>상태</td><td>상담사 상태(로그 아웃, 휴식 중, 대기 중, 통화 중, 후 처리)</td></tr><tr><td>상태 사유</td><td>상담사 상태별 세부 사유까지 표시</td></tr><tr><td>유지 시간</td><td>상담사 해당 상태로 유지된 시간</td></tr><tr><td>내선</td><td>상담사가 사용하고 있는 전화번호</td></tr><tr><td>미디어 로그인ID</td><td>상담사의 전화기에 할당된 미디어 로그인 ID (일반적으로 내선번호와 동일하게 설정)</td></tr><tr><td>Blend종류</td><td>상담사 업무 구분(Inbound, Outbound, Blend)</td></tr></tbody></table>



### 대시 보드 <a href="#dashboard" id="dashboard"></a>

대시보드 페이지는 라우트/큐 현황, 대기호, 상담사 리스트를 한 화면에 보여줍니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EB%8C%80%EC%8B%9C%20%EB%B3%B4%EB%93%9C.png" alt=""><figcaption><p>모니터링 대시 보드</p></figcaption></figure>

**라우트 / 큐**

라우트/큐 항목은 큐별 대기호 수, 총 인입 수, 서비스 레벨, 분배호, 포기호를 보여줍니다.

<table><thead><tr><th width="172">구분</th><th>설명</th></tr></thead><tbody><tr><td>서비스 레벨</td><td>일정한 시간 안에 응답되거나 포기된 호의 비율</td></tr><tr><td>응답율</td><td>큐에 인입된 호 중 상담원에게 분배된 호의 비율<br>(응답률 = 응답호수 / 인입호수 * 100)</td></tr><tr><td>대기호</td><td>큐에 인입 후 상담원에게 분배되기 위해 대기 중인 호</td></tr><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐 ID</td><td>큐 ID</td></tr><tr><td>큐 이름</td><td>큐 이름</td></tr><tr><td>대기호</td><td>큐에 인입 후 상담원에게 분배되기 위해 대기중인 호</td></tr><tr><td>총 인입호</td><td>큐에 인입된 총 호수</td></tr><tr><td>서비스 레벨(%)</td><td>일정한 시간 안에 응답되거나 포기된 호의 비율</td></tr><tr><td>분배호</td><td>큐에 인입 후 상담원에 분배되어 응답한 호수</td></tr><tr><td>포기호</td><td>큐에 인입 후 상담원에게 분배되기 전 설정한 대기시간 이내에 고객이 끊은 호수</td></tr></tbody></table>

**대기호**

대기호 현황을 확인할 수 있습니다.

**상담사**

상담사 항목은 상담사별 상태, 상태 사유, 유지 시간 등을 리스트 형식으로 보여줍니다. 콜 상담과 채팅 상담으로 구분하여 조회도 가능합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EB%8C%80%EC%8B%9C%20%EB%B3%B4%EB%93%9C%20%EC%83%81%EB%8B%B4%EC%82%AC.png" alt=""><figcaption><p>모니터링 대시 보드 상담사</p></figcaption></figure>

<table><thead><tr><th width="179">구분</th><th>설명</th></tr></thead><tbody><tr><td>대기</td><td>상담사 상태가 대기로 설정된 상담사 수</td></tr><tr><td>휴식</td><td>상담사 상태가 휴식으로 설정된 상담사 수</td></tr><tr><td>통화중</td><td>상담사 상태가 통화 중인 상담사 수</td></tr><tr><td>후처리</td><td>상담사 상태가 후 처리 중인 상담사 수</td></tr><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>상담사 ID</td><td>상담사 ID</td></tr><tr><td>상담사</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 그룹 ID, 상담사 그룹 이름</td></tr><tr><td>팀</td><td>상담사 팀 ID, 상담사 팀 이름</td></tr><tr><td>상태</td><td>상담사 상태(로그 아웃</td></tr><tr><td>상태 사유</td><td>상담사 상태별 세부 사유까지 표시</td></tr><tr><td>유지 시간</td><td>상담사 현재 상태로 유지된 시간</td></tr><tr><td>내선</td><td>상담원이 사용하고 있는 전화번호</td></tr></tbody></table>

**자원 범위 설정**

대시보드, 대기호, 상담사 화면에 대해서 갱신 주기 또는 자원 범위를 지정할 수 있습니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EC%9E%90%EC%9B%90%20%EB%B2%94%EC%9C%84%20%EC%84%A4%EC%A0%95.png" alt=""><figcaption><p>모니터링 자원 범위 설정</p></figcaption></figure>

### 라우트 / 큐 <a href="#route-que" id="route-que"></a>

라우트/큐 페이지는 라우트/큐에 대한 모니터링 화면을 보여줍니다. 현재 컨택센터의 서비스 레벨(%), 응답률(%), 대기호 정보가 실시간 표시되어 효과적인 모니터링이 가능합니다. 그 외에 총 인입호 수, 실 인입호 수 등의 통계가 실시간으로 표시되어 컨택센터 관리자의 의사 결정에 도움을 줍니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EB%9D%BC%EC%9A%B0%ED%8A%B8%20%ED%81%90.png" alt=""><figcaption><p>모니터링 라우트 큐</p></figcaption></figure>

**자원 범위 설정**

모니터링 하고자 하는 테넌트, 큐 대분류, 큐 중분류, 큐를 선택 후 조회 버튼을 클릭합니다.

테넌트는 1개만 선택이 가능하며 큐 대분류, 큐 중분류, 큐는 ALL 선택이 가능합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EB%9D%BC%EC%9A%B0%ED%8A%B8%20%ED%81%90%20%EC%9E%90%EC%9B%90%20%EB%B2%94%EC%9C%84.png" alt=""><figcaption><p>모니터링 라우트 큐 자원 범위</p></figcaption></figure>



**라우트 현황**

IVR 채널별로 상태(IDLE,BUSY)를 그래프로 제공합니다.

<table><thead><tr><th width="181">구분</th><th>설명</th></tr></thead><tbody><tr><td>서비스 레벨</td><td>큐에 인입 되어 일정한 시간 안에 응답되거나 포기된 호의 비율</td></tr><tr><td>응답율</td><td>큐에 인입된 호 중 상담원에게 분배된 호의 비율 (응답률 = 응답호수 / 실 인입호수 * 100)</td></tr><tr><td>대기호</td><td>큐에 인입 후 상담원에게 분배 되기 위해 대기 중인 호</td></tr><tr><td>총인입</td><td>큐에 인입된 총 호수 (실 인입 + 타 센터 라우팅 + 그룹호 전환 + 큐 전환)</td></tr><tr><td>실인입 호수</td><td>큐에 인입된 호 중 유효한(타 센터 라우팅, 재 인입된 호 제외) 호의 수</td></tr><tr><td>상담사 분배호수</td><td>큐에 인입 후 상담원에 분배 되어 응답한 호수</td></tr><tr><td>포기호</td><td>큐에 인입 후 상담원에게 분배 되기 전 설정한 대기 시간 이내에 고객이 끊은 호수</td></tr><tr><td>넌 서비스 호수</td><td>큐에 인입 후 CTI 시스템에서 설정한 최대 대기 시간을 초과하여 끊어진 호수<br>(큐에 인입 되었으나 일정 시간이 초과한 후 분배 되지 않고 끊긴 호의 수 + 외부 호 전환된 호의 수)</td></tr><tr><td>콜백</td><td>큐에 인입 후 콜백 큐로 넘어간 호수.</td></tr><tr><td>큐 전환</td><td>큐에 인입 후 다른 큐, IVRDN, 외부 등 상담원DN을 제외한 DN으로 넘어간 호수</td></tr><tr><td>실패</td><td>큐에 인입된 호 중 분배 명령이 이루어진 시점에 물리적인 이유로 인해 분배 하려던 상담석 전화로 연결할 수 없어 끊어진 호수</td></tr><tr><td>그룹호 전환</td><td>그룹호 전환 되어 상담원에게 분배 된 호수</td></tr><tr><td>타 센터 라우팅</td><td>타 센터로 라우팅 된 호수</td></tr><tr><td>터 센터 라우팅 실패</td><td>타 센터로 라우팅 됐지만 실패된 호수</td></tr><tr><td>타 센터 인입</td><td>타 센터로부터 인입된 호수</td></tr></tbody></table>

**큐 모니터링 리스트**

큐 모니터 리스트 항목에는 큐 각각의 상태 및 통계를 모니터링 기능을 제공합니다.

<table><thead><tr><th width="183">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐 ID</td><td>큐 ID</td></tr><tr><td>큐 이름</td><td>큐 이름</td></tr><tr><td>대기호</td><td>현재 큐에 대기중인 호수의 합</td></tr><tr><td>현재 최대 대기시간</td><td>현재 큐에 인입된 콜 중 최대 대기 시간</td></tr><tr><td>금일 최대 대기시간</td><td>금일 큐에 인입된 콜 중 최대 대기 시간</td></tr><tr><td>총 인입호</td><td>큐에 들어온 총 인입 호수</td></tr><tr><td>서비스 레벨</td><td>큐의 현재 서비스 레벨</td></tr><tr><td>분배호</td><td>큐에 들어온 후 상담사 분배된 호수</td></tr><tr><td>실패호</td><td>큐에 인입 되어 분배 되었으나 물리적인 이유로 인해 분배 받은 상담사와 연결이 되지 않아 끊어진 호의 수</td></tr><tr><td>포기호</td><td>큐에 들어온 후 고객이 전화를 끊은 호수</td></tr></tbody></table>



### 대기호 <a href="#waiting" id="waiting"></a>

대기호 페이지에는 대기호 현황에 대한 모니터링 화면을 보여줍니다. 현재 컨택센터의 대기호 정보가 막대 그래프로 실시간 표시되어 효과적인 모니터링이 가능합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EB%8C%80%EA%B8%B0%ED%98%B8.png" alt=""><figcaption><p>모니터링 대기호</p></figcaption></figure>

**자원 범위**

모니터링 하고자 하는 테넌트, 대분류, 중분류, 큐 선택 후 조회 버튼을 클릭합니다.

**대기호 현황**

대기호(인바운드 상담전화가 착신이 되었으나 상담원에게 연결되지 않은 호)를 대기 시간별로 표시합니다. 대기호를 20초, 30초, 60초 간격으로 구분하여 조회를 할 수 있고 대기호 시간이 길어짐에 따라 그래프가 이동됩니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EB%8C%80%EA%B8%B0%ED%98%B8%20%ED%98%84%ED%99%A9.png" alt=""><figcaption><p>모니터링 대기호 현황</p></figcaption></figure>

**대기호 리스트**

대기호 리스트 항목에는 큐별 대기호 현황을 제공합니다. 대기호 시간이 길어짐에 따라 시간대별로 대기호의 수가 변화됨을 확인할 수 있습니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EB%8C%80%EA%B8%B0%ED%98%B8%20%EB%A6%AC%EC%8A%A4%ED%8A%B8.png" alt=""><figcaption><p>모니터링 대기호 리스트</p></figcaption></figure>

<table><thead><tr><th width="195">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐 ID</td><td>큐 ID</td></tr><tr><td>큐 이름</td><td>큐 이름</td></tr><tr><td>시간대 1~20</td><td>큐에 인입된 호 중 대기시간이 1~20초 이내인 콜 수</td></tr><tr><td>시간대 21~40</td><td>큐에 인입된 호 중 대기시간이 21~40초 이내인 콜 수</td></tr><tr><td>시간대 41~60</td><td>큐에 인입된 호 중 대기시간이 41~60초 이내인 콜 수</td></tr><tr><td>시간대 61~80</td><td>큐에 인입된 호 중 대기시간이 61~80초 이내인 콜 수</td></tr><tr><td>시간대 81~300</td><td>큐에 인입된 호 중 대기시간이 81~300초 이내인 콜 수</td></tr><tr><td>시간대 301~</td><td>큐에 인입된 호 중 대기시간이 301초 이상인 콜 수</td></tr></tbody></table>

### 대기호 상세 <a href="#waiting-details" id="waiting-details"></a>

대기호 상세 페이지에는 대기호에 대하여 콜/채팅을 구분하여 모니터링 현황을 보여줍니다. 현재 컨택센터의 대기호 정보가 막대 그래프로 실시간 표시되어 효과적인 모니터링 할 수 있습니다.

**자원 범위**

모니터링 하고자 하는 테넌트, 옴니채널(Call / Chat)을 선택 후 조회합니다.

**대기호 상세**

대기호(인바운드 상담전화가 착신이 되었으나 상담원에게 연결되지 않은 호)를 대기 시간별로 표시합니다. 대기호를 20초, 30초, 60초 간격으로 구분하여 조회할 수 있고 대기호 시간이 길어짐에 따라 그래프가 이동됩니다.

**대기호 상세 리스트**

대기호 리스트 항목에는 큐별 대기호 현황을 제공합니다. 대기호 시간이 길어짐에 따라 시간대별로 대기호의 수가 변화됨을 확인할 수 있습니다.

<table><thead><tr><th width="160">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐ID</td><td>큐 ID</td></tr><tr><td>큐 이름</td><td>큐 이름</td></tr><tr><td>콜 ID</td><td>콜 ID</td></tr><tr><td>CNID</td><td>중복되지 않는 관리용 고유번호</td></tr><tr><td>고객번호</td><td>큐에서 대기 중인 고객의 전화번호</td></tr><tr><td>우선순위</td><td>대기호의 우선 순위로, 우선순위를 가져야 할 고객의 분배 순위를 높일 때 표현</td></tr><tr><td>대기시간</td><td>큐에서 대기한 시간</td></tr><tr><td>옴니 채널</td><td>인입된 채널 종류 ( call / chat )</td></tr><tr><td>콜타입</td><td>I/B 통화</td></tr><tr><td>사용자 정보</td><td>사용자 관련 정보</td></tr><tr><td>대표번호</td><td>DNIS</td></tr></tbody></table>



### 상담사 <a href="#counselor" id="counselor"></a>

상담사에 대한 모니터링 화면을 보여줍니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81%20%EC%83%81%EB%8B%B4%EC%82%AC.png" alt=""><figcaption><p>모니터링 상담사</p></figcaption></figure>

**자원 범위**

모니터링 하고자 하는 테넌트, 그룹, 팀 선택 후 \[조회] 버튼을 클릭합니다.

**상담사 상태**

<table><thead><tr><th width="154">구분</th><th>설명</th></tr></thead><tbody><tr><td>상담사 상태</td><td><p>대기: 상담사 상태가 대기인 상담사 수 <br>휴식: 상담사 상태가 휴식인 상담사 수 <br>통화 중: 상담사 상태가 통화중인 상담사 수 <br>후처리: 상담사 상태가 후처리인 상담사 수</p><ul><li>상담사 1명이 콜상담과 채팅 상담 모두에 대해서 휴식 상태로 설정될 경우 총 5건 휴식 ( 콜상담=1건, 채팅상담=4건)으로 표시됨(2022.08)</li></ul></td></tr><tr><td>휴식 사유 실시간</td><td>일반 휴식: 상담사 상태가 휴식(일반휴식) <br>개인 테스트: 상담사 상태가 휴식(개인) <br>식사: 상담사 상태가 휴식(식사) <br>티타임: 상담사 상태가 휴식(티타임) <br>교육: 상담사 상태가 휴식(교육) <br>회의: 상담사 상태가 휴식(회의) <br>상담: 상담사 상태가 휴식(상담) <br>다른 업무: 상담사 상태가 휴식(다른 업무) <br>개인 업무: 상담사 상태가 휴식(개인 업무) <br>수리: 상담사 상태가 휴식(수리)</td></tr></tbody></table>

<table><thead><tr><th width="171">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>상담사 ID</td><td>상담사 ID</td></tr><tr><td>상담사</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 그룹 ID, 상담사 그룹 이름</td></tr><tr><td>팀</td><td>상담사 팀 ID, 상담사 파트 이름</td></tr><tr><td>상태</td><td>상담사 상태(로그 아웃, 휴식 중, 대기 중, 통화 중, 후 처리)</td></tr><tr><td>모니터링</td><td>현재 통화 상태인 상담사의 통화 내용 실시간 청취</td></tr><tr><td>상태사유</td><td>상담사 상태 사유명 변경 가능하고 최대 10개까지 설정 가능</td></tr><tr><td>유지시간</td><td>상담사 현재 상태로 유지된 시간</td></tr><tr><td>상태변경</td><td>상담사 상태를 강제로 변경</td></tr><tr><td>내선</td><td>상담사가 사용하고 있는 전화번호</td></tr><tr><td>미디어 로그인ID</td><td>상담사의 전화기에 할당된 미디어 로그인 ID (일반적으로 내선번호와 동일하게 설정)</td></tr><tr><td>스킬 분배</td><td>콘솔에서 작성한 상담 스킬</td></tr><tr><td>Blend종류</td><td>상담사 업무 구분(Inbound, Outbound, Blend)</td></tr></tbody></table>

* 상담사 상태 강제 변경은 로그인한 상담사 계정만 상태 변경 메뉴가 활성화됩니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%EC%82%AC%20%EC%83%81%ED%83%9C%20%EA%B0%95%EC%A0%9C%20%EB%B3%80%EA%B2%BD.png" alt=""><figcaption><p>상담사 상태 강제 변경</p></figcaption></figure>
