# 통계

## 통계 - 큐 <a href="#stats-que" id="stats-que"></a>

자원에 대한 통계를 제공합니다.

### 큐 실적(건수)

총합 / 분대별 / 시간대별 / 요일별 / 일별 / 월별 / 년도별로 큐 실적을 건수로 보여줍니다.

**총합**

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%ED%81%90%20%EC%8B%A4%EC%A0%81%20%EA%B1%B4%EC%88%98.png" alt=""><figcaption><p>큐 실적 건수</p></figcaption></figure>

<table><thead><tr><th width="155">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐</td><td>큐 일련번호</td></tr><tr><td>큐이름</td><td>큐 이름</td></tr><tr><td>그룹</td><td>큐 소속 그룹</td></tr><tr><td>팀</td><td>큐 소속 팀</td></tr><tr><td>인입 구분</td><td>큐 인입 구분</td></tr><tr><td>콜타입</td><td>큐 인입시 콜 타입</td></tr><tr><td>상담 채널</td><td>연결 미디어 타입</td></tr><tr><td>총인입</td><td>큐에 인입된 총 호수의 합 (실 인입 + 타 센터 라우팅 + 그룹호전환 + 큐 전환)</td></tr><tr><td>실인입</td><td>큐에 실인입된 총 호수의 합 (응답호수 + 포기호수 + 넌서비스 + 실패 + 콜백 + 외부호전환) (실 인입 + 타 센터 라우팅 + 그룹호전환 + 큐 전환)</td></tr><tr><td>분배호수</td><td>큐에 인입 후 상담원에 분배된 호수의 합</td></tr><tr><td>포기호수</td><td>큐에 인입 후 상담원에게 분배되기 전 고객이 끊은 호수의 합</td></tr><tr><td>넌서비스</td><td>큐에 인입 후 CTI 시스템에서 설정한 최대 대기 시간을 초과하여 끊어진 호수의 합</td></tr><tr><td>실패</td><td>큐에 인입된 호 중 분배 명령이 이루어진 시점에 물리적인 이유로 인해 분배 하려던 상담석 전화로 연결할 수 없어 끊어진 호수의 합</td></tr><tr><td>외부호 전환</td><td>큐에 인입된 호 중 외부로 호 전환한 호수의 합</td></tr><tr><td>콜백</td><td>큐에 인입 후 콜백 큐로 넘어간 호수의 합</td></tr><tr><td>큐실적(전환)</td><td>큐에 인입 후 다른 큐, IVRDN, 외부 등 상담원DN을 제외한 DN으로 넘어간 호수의 합</td></tr></tbody></table>

### 큐 실적(총합)

총합 / 분대별 / 시간대별 / 요일별 / 일별 / 월별 / 년도별로 큐 실적을 조회합니다.

**총합**

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%ED%81%90%20%EC%8B%A4%EC%A0%81%20%EC%B4%9D%ED%95%A9.png" alt=""><figcaption><p>큐 실적 총합</p></figcaption></figure>

<table><thead><tr><th width="180">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐</td><td>큐 일련번호</td></tr><tr><td>큐 이름</td><td>큐 이름</td></tr><tr><td>그룹</td><td>큐 소속 그룹</td></tr><tr><td>팀</td><td>큐 소속 팀</td></tr><tr><td>인입 구분</td><td>큐 인입 구분</td></tr><tr><td>콜타입</td><td>큐 인입시 콜 타입</td></tr><tr><td>상담 채널</td><td>연결 미디어 타입</td></tr><tr><td>총인입 총호수</td><td>큐에 인입된 총 호수의 합 (실 인입 + 타 센터 라우팅 + 그룹호 전환 + 큐 전환)</td></tr><tr><td>총인입 총점유</td><td>큐에 인입된 총 호수의 점유 시간 (실 인입 + 타 센터 라우팅 + 그룹호 전환 + 큐 전환)</td></tr><tr><td>총인입 %</td><td>큐에 인입된 총 호수의 비율 (실 인입 + 타 센터 라우팅 + 그룹호 전환 + 큐 전환)</td></tr><tr><td>총인입 평균점유</td><td>큐에 인입된 총 호수의 평균 점유 시간 (실 인입 + 타 센터 라우팅 + 그룹호 전환 + 큐 전환)</td></tr><tr><td>실인입 총호수</td><td>큐에 실 인입된 총 호수의 합 (응답호 수 + 포기호 수 + 넌서비스 + 실패 + 콜백 + 외부호 전환) (실 인입 + 타 센터 라우팅 + 그룹호 전환 + 큐 전환)</td></tr><tr><td>실인입 총점유</td><td>큐에 실 인입된 총 호수의 점유 시간 (응답호 수 + 포기호 수 + 넌서비스 + 실패 + 콜백 + 외부호 전환) (실 인입 + 타 센터 라우팅 + 그룹호전환 + 큐 전환)</td></tr><tr><td>실인입 %</td><td>큐에 실 인입된 총 호수의 비율 (응답호 수 + 포기호 수 + 넌서비스 + 실패 + 콜백 + 외부호 전환) (실 인입 + 타 센터 라우팅 + 그룹호 전환 + 큐 전환)</td></tr><tr><td>실인입 평균점유</td><td>큐에 실 인입된 총 호수의 평균 점유 시간 (응답호 수 + 포기호 수 + 넌서비스 + 실패 + 콜백 + 외부호 전환) (실 인입 + 타 센터 라우팅 + 그룹호 전환 + 큐 전환)</td></tr><tr><td>분배호 수 총호수</td><td>큐에 인입 후 상담사에 분배된 호수의 합</td></tr><tr><td>분배호 수 총점유</td><td>큐에 인입 후 상담사에 분배된 호수의 점유 시간</td></tr><tr><td>분배호 수 %</td><td>큐에 인입 후 상담사에 분배된 호수의 비율</td></tr><tr><td>분배호 수 평균점유</td><td>큐에 인입 후 상담사에 분배된 호수의 평균 점유 시간</td></tr><tr><td>포기호 수 총 호수</td><td>큐에 인입 후 상담사에게 분배되기 전 고객이 끊은 호수의 합</td></tr><tr><td>포기호 수 총 점유</td><td>큐에 인입 후 상담사에게 분배되기 전 고객이 끊은 호수의 점유시간</td></tr><tr><td>포기호 수 %</td><td>큐에 인입 후 상담사에게 분배되기 전 고객이 끊은 호수의 비율</td></tr><tr><td>포기호수 평균 점유</td><td>큐에 인입 후 상담사에게 분배되기 전 고객이 끊은 호수의 평균 점유 시간</td></tr><tr><td>넌서비스 총호수</td><td>큐에 인입 후 CTI 시스템에서 설정한 최대 대기 시간을 초과하여 끊어진 호수의 합</td></tr><tr><td>넌서비스 총점유</td><td>큐에 인입 후 CTI 시스템에서 설정한 최대 대기 시간을 초과하여 끊어진 호수의 점유 시간</td></tr><tr><td>넌서비스 %</td><td>큐에 인입 후 CTI 시스템에서 설정한 최대 대기 시간을 초과하여 끊어진 호수의 비율</td></tr><tr><td>넌서비스 평균점유</td><td>큐에 인입 후 CTI 시스템에서 설정한 최대 대기 시간을 초과하여 끊어진 호수의 평균 점유 시간</td></tr><tr><td>실패 총 호수</td><td>큐에 인입된 호 중 분배 명령이 이루어진 시점에 물리적인 이유로 인해 분배 하려던 상담석 전화로 연결할 수 없어 끊어진 호수의 합</td></tr><tr><td>실패 총 점유</td><td>큐에 인입된 호 중 분배 명령이 이루어진 시점에 물리적인 이유로 인해 분배 하려던 상담석 전화로 연결할 수 없어 끊어진 호수의 점유 시간</td></tr><tr><td>실패 %</td><td>큐에 인입된 호 중 분배 명령이 이루어진 시점에 물리적인 이유로 인해 분배 하려던 상담석 전화로 연결할 수 없어 끊어진 호수의 비율</td></tr><tr><td>실패 평균 점유</td><td>큐에 인입된 호 중 분배 명령이 이루어진 시점에 물리적인 이유로 인해 분배 하려던 상담석 전화로 연결할 수 없어 끊어진 호수의 평균 점유 시간</td></tr><tr><td>외부호 전환 총호수</td><td>큐에 인입된 호중 외부로 호 전환한 호수의 합</td></tr><tr><td>외부호 전환 총점유</td><td>큐에 인입된 호중 외부로 호 전환한 호수의 점유 시간</td></tr><tr><td>콜백 총 호수</td><td>큐에 인입 후 콜백 큐로 넘어간 호수의 합</td></tr><tr><td>콜백 총 점유</td><td>큐에 인입 후 콜백 큐로 넘어간 호수의 점유 시간</td></tr><tr><td>큐실적(전환) 총호수</td><td>큐에 인입 후 다른 큐, IVRDN, 외부 등 상담원DN을 제외한 DN으로 넘어간 호수의 합</td></tr><tr><td>큐실적(전환) 총점유</td><td>큐에 인입 후 다른 큐, IVRDN, 외부 등 상담원DN을 제외한 DN으로 넘어간 호수의 점유 시간</td></tr><tr><td>타 센터 인입 총 호수</td><td>타 센터로부터 인입된 호수의 합</td></tr><tr><td>타 센터 인입 총 점유</td><td>타 센터로부터 인입된 호수의 점유 시간</td></tr><tr><td>타 센터 라우팅 성공</td><td>타 센터로 라우팅된 호 중에서 타센터 상담원에게 분배된 호수</td></tr><tr><td>타 센터 라우팅 실패</td><td>타 센터로 라우팅된 호 중에서 실패된 호수</td></tr><tr><td>서비스레벨</td><td>일정한 시간 안에 응답 되거나 포기된 호의 비율</td></tr><tr><td>서비스레벨 건수</td><td>일정한 시간 안에 응답 되거나 포기된 호의 건수</td></tr></tbody></table>



### 큐 5초 단위 분배

총합 / 분대별 / 시간대별 / 요일별 / 일별 / 월별 / 년도별로 큐에 인입된 호에 대해서 5초 단위로 분배된 카운터를 조회합니다.

**총합**

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%ED%81%90%205%EC%B4%88%20%EB%8B%A8%EC%9C%84%20%EB%B6%84%EB%B0%B0.png" alt=""><figcaption><p>큐 5초 단위 분배</p></figcaption></figure>

<table><thead><tr><th width="182">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐</td><td>큐 일련번호</td></tr><tr><td>큐 이름</td><td>큐 이름</td></tr><tr><td>그룹</td><td>큐 소속 그룹</td></tr><tr><td>팀</td><td>큐 소속 팀</td></tr><tr><td>콜타입</td><td>큐 인입시 콜 타입</td></tr><tr><td>분배 n~n초</td><td>해당 시간내 분배된 호수</td></tr><tr><td>총 분배</td><td>전체 분배된 호수</td></tr></tbody></table>

### 큐 5초 단위 포기

총합 / 분대별 / 시간대별 / 요일별 / 일별 / 월별 / 년도별로 큐에 인입된 호에 대해서 5초 단위로 포기한 카운터를 조회합니다.

**총합**

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%ED%81%90%205%EC%B4%88%20%EB%8B%A8%EC%9C%84%20%ED%8F%AC%EA%B8%B0.png" alt=""><figcaption><p>큐 5초 단위 포기</p></figcaption></figure>

<table><thead><tr><th width="156">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 명</td></tr><tr><td>큐</td><td>큐 일련번호</td></tr><tr><td>큐이름</td><td>큐 이름</td></tr><tr><td>그룹</td><td>큐 소속 그룹</td></tr><tr><td>팀</td><td>큐 소속 팀</td></tr><tr><td>콜타입</td><td>큐 인입시 콜 타입</td></tr><tr><td>포기 n~n초</td><td>해당 시간내 포기된 호수</td></tr><tr><td>총 포기</td><td>전체 포기된 호수</td></tr></tbody></table>



### 포기호 리스트

포기호 리스트를 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%ED%8F%AC%EA%B8%B0%ED%98%B8%20%EB%A6%AC%EC%8A%A4%ED%8A%B8.png" alt=""><figcaption><p>포기호 리스트</p></figcaption></figure>

<table><thead><tr><th width="162">구분</th><th>설명</th></tr></thead><tbody><tr><td>순번</td><td>순번</td></tr><tr><td>마감 일자</td><td>큐 포기된 일자</td></tr><tr><td>인입 시간</td><td>큐 인입된 시간</td></tr><tr><td>포기 시간</td><td>큐 포기된 시간</td></tr><tr><td>대기 시간</td><td>큐 인입 부터 포기까지 대기 시간</td></tr><tr><td>큐ID</td><td>큐 일련번호</td></tr><tr><td>큐 이름</td><td>큐 이름</td></tr><tr><td>전화번호</td><td>고객 전화 번호</td></tr></tbody></table>



## 통계 - 상담사 <a href="#stats-counselor" id="stats-counselor"></a>

### 상담 실적(건수)

상담사 실적을 건수 형태로 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%20%EC%8B%A4%EC%A0%81%20%EA%B1%B4%EC%88%98.png" alt=""><figcaption><p>상담 실적 건수</p></figcaption></figure>

**자원 범위**

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%20%EC%8B%A4%EC%A0%81%20%EA%B1%B4%EC%88%98%20%EC%9E%90%EC%9B%90%20%EB%B2%94%EC%9C%84.png" alt=""><figcaption><p>상담 실적 건수 자원 범위</p></figcaption></figure>

자원 범위 선택 시 테넌트는 1개만 선택 가능하고 해당 테넌트에 소속된 1개 이상의 그룹을 지정해야 합니다.

<table><thead><tr><th width="126">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 이름</td></tr><tr><td>상담사 ID</td><td>상담사 일련번호</td></tr><tr><td>상담사명</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 소속 그룹</td></tr><tr><td>팀</td><td>상담사 소속 팀</td></tr><tr><td>상담 채널</td><td>연결 미디어 타입</td></tr><tr><td>총통화</td><td>상담사에게 분배되어 고객과 상담원간의 통화가 이루어진 상태의 총 통화<br><code>총통화 = I/B통화 + O/B통화 + 내부 통화(받은, 보낸) + 협의 통화(보낸, 받은) + 전환 통화(받은, 보낸) + 회의 통화(받은, 보낸)</code></td></tr><tr><td>I/B 접속</td><td>통화와는 관계없이 인바운드로 연결 된 전체 통화 호수</td></tr><tr><td>I/B 통화</td><td>고객으로부터 상담사와 연결된 통화로서 PSTN을 통한 인바운드 통화</td></tr><tr><td>O/B 접속</td><td>통화와는 관계없이 상담사가 외부로 연결한 전체 통화 호수</td></tr><tr><td>O/B 통화</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화</td></tr><tr><td>보낸 그룹호</td><td>상담사가 통화 중 큐 혹은 다른 상담 그룹, 팀에게 보낸 그룹 호수</td></tr><tr><td>받은 그룹호</td><td>상담사가 다른 상담사게 보낸 그룹 호를 받은 그룹 호수</td></tr><tr><td>보낸 내부</td><td>컨택 센터 내부에서 상담사로 보낸 통화</td></tr><tr><td>받은 내부</td><td>컨택 센터 내부에서 상담사로 받은 통화</td></tr><tr><td>보낸 협의</td><td>상담사가 통화 중 다른 상담원과의 협의를 위해 내선에서 다른 상담사나 외부 전화로 보낸 통화</td></tr><tr><td>받은 협의</td><td>상담사가 통화 중 다른 상담원과의 협의를 위해 내선에서 다른 상담사나 외부 전화로 받은 통화</td></tr><tr><td>보낸 전환</td><td>상담사나 큐로 부터 다른 상담사나 큐로 보낸 전환 연결된 통화</td></tr><tr><td>받은 전환</td><td>상담사나 큐로 부터 다른 상담사나 큐에서 받은 전환 통화</td></tr><tr><td>보낸 회의</td><td>3명 이상의 다자간 통화 중 보낸 회의 통화</td></tr><tr><td>받은 회의</td><td>3명 이상의 다자간 통화 중 받은 회의 통화</td></tr><tr><td>직접 인입</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수</td></tr></tbody></table>



### 상담 실적(통화)

상담사 실적을 통화 형태로 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%20%EC%8B%A4%EC%A0%81%20%ED%86%B5%ED%99%94.png" alt=""><figcaption><p>상담 실적 통화</p></figcaption></figure>

<table><thead><tr><th width="161">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 이름</td></tr><tr><td>상담사ID</td><td>상담사 일련번호</td></tr><tr><td>상담사명</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 소속 그룹</td></tr><tr><td>팀</td><td>상담사 소속 팀</td></tr><tr><td>상담 채널</td><td>연결 미디어 타입</td></tr><tr><td>총 통화 횟수</td><td>상담사에게 분배 되어 고객과 상담사간의 통화가 이루어진 상태의 총 통화 횟수</td></tr><tr><td>총 통화 시간</td><td>상담사에게 분배 되어 고객과 상담사간의 통화가 이루어진 상태의 총 통화 시간</td></tr><tr><td>총 통화 - %</td><td>상담사에게 분배 되어 고객과 상담사간의 통화가 이루어진 상태의 총 통화 비율</td></tr><tr><td>총 통화 - 평균</td><td>상담사에게 분배 되어 고객과 상담사간의 통화가 이루어진 상태의 총 통화 평균 시간</td></tr><tr><td>I/B통화 횟수</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인 바운드 통화 횟수</td></tr><tr><td>I/B통화 시간</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인 바운드 통화 시간</td></tr><tr><td>I/B통화 - %</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인 바운드 통화 비율</td></tr><tr><td>I/B통화 - 평균</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인 바운드 통화 평균 시간</td></tr><tr><td>O/B통화 횟수</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화 횟수</td></tr><tr><td>O/B통화 시간</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화 시간</td></tr><tr><td>O/B통화 - %</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화 비율</td></tr><tr><td>O/B통화 - 평균</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화 평균 시간</td></tr><tr><td>내부 통화 횟수</td><td>컨택 센터 내부에 등록된 상담사나 큐 간의 통화 횟수</td></tr><tr><td>내부 통화 시간</td><td>컨택 센터 내부에 등록된 상담사나 큐 간의 통화 시간</td></tr><tr><td>내부 통화 - %</td><td>컨택 센터 내부에 등록된 상담사나 큐 간의 통화 비율</td></tr><tr><td>내부 통화 - 평균</td><td>컨택 센터 내부에 등록된 상담사나 큐 간의 통화 평균 시간</td></tr><tr><td>협의 통화 횟수</td><td>상담사가 통화 중 다른 상담사와 협의를 위해 내선에서 다른 상담사나 외부 전화로 연결된 통화 횟수</td></tr><tr><td>협의 통화 시간</td><td>상담사가 통화 중 다른 상담사와 협의를 위해 내선에서 다른 상담사나 외부 전화로 연결된 통화 시간</td></tr><tr><td>협의 통화 - %</td><td>상담사가 통화 중 다른 상담사와 협의를 위해 내선에서 다른 상담사나 외부 전화로 연결된 통화 비율</td></tr><tr><td>협의 통화 - 평균</td><td>상담사가 통화 중 다른 상담사와 협의를 위해 내선에서 다른 상담사나 외부 전화로 연결된 통화 평균 시간</td></tr><tr><td>전환 통화 횟수</td><td>상담사나 큐로 부터 다른 상담사나 큐로 전환 연결된 통화 횟수</td></tr><tr><td>전환 통화 시간</td><td>상담사나 큐로 부터 다른 상담사나 큐로 전환 연결된 통화 시간</td></tr><tr><td>전환 통화 - %</td><td>상담사나 큐로 부터 다른 상담사나 큐로 전환 연결된 통화 비율</td></tr><tr><td>전환통화 - 평균</td><td>상담사나 큐로 부터 다른 상담사나 큐로 전환 연결된 통화 평균 시간</td></tr><tr><td>회의 통화 횟수</td><td>3명 이상의 다자간 통화 횟수 (흔히 고객, 담당 상담사, 매니저 상담사의 3자 통화)</td></tr><tr><td>회의 통화 시간</td><td>3명 이상의 다자간 통화 시간 (흔히 고객, 담당 상담사, 매니저 상담사의 3자 통화)</td></tr><tr><td>회의 통화 - %</td><td>3명 이상의 다자간 통화 비율 (흔히 고객, 담당 상담사, 매니저 상담사의 3자 통화)</td></tr><tr><td>회의 통화 - 평균</td><td>3명 이상의 다자간 통화 평균 시간 (흔히 고객, 담당 상담사, 매니저 상담사의 3자 통화)</td></tr><tr><td>직접 인입 횟수</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수의 횟수</td></tr><tr><td>직접 인입 시간</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수의 시간</td></tr><tr><td>직접 인입 - %</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수의 비율</td></tr><tr><td>직접 인입 - 평균</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수의 평균 시간</td></tr></tbody></table>

### 상담 실적(총합)

상담사별 실적 (총합) 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%20%EC%8B%A4%EC%A0%81%20%EC%B4%9D%ED%95%A9.png" alt=""><figcaption><p>상담 실적 총합</p></figcaption></figure>

<table><thead><tr><th width="160">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 이름</td></tr><tr><td>상담사ID</td><td>상담사 일련번호</td></tr><tr><td>상담사명</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 소속 그룹</td></tr><tr><td>팀</td><td>상담사 소속 팀</td></tr><tr><td>상담 채널</td><td>연결 미디어 타입</td></tr><tr><td>총 통화 횟수</td><td>상담사에게 분배 되어 고객과 상담사간의 통화가 이루어진 상태의 총 통화 횟수</td></tr><tr><td>총 통화 시간</td><td>상담사에게 분배 되어 고객과 상담사간의 통화가 이루어진 상태의 총 통화 시간</td></tr><tr><td>총 통화 - %</td><td>상담사에게 분배 되어 고객과 상담사간의 통화가 이루어진 상태의 총 통화 비율</td></tr><tr><td>총 통화 - 평균</td><td>상담사에게 분배 되어 고객과 상담사간의 통화가 이루어진 상태의 총 통화 평균 시간</td></tr><tr><td>I/B통화 횟수</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인 바운드 통화 횟수</td></tr><tr><td>I/B통화 시간</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인 바운드 통화 시간</td></tr><tr><td>I/B통화 - %</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인 바운드 통화 비율</td></tr><tr><td>I/B통화 - 평균</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인 바운드 통화 평균 시간</td></tr><tr><td>O/B통화 횟수</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화 횟수</td></tr><tr><td>O/B통화 시간</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화 시간</td></tr><tr><td>O/B통화 - %</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화 비율</td></tr><tr><td>O/B통화 - 평균</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃 바운드 통화 평균 시간</td></tr><tr><td>내부 통화 횟수</td><td>컨택 센터 내부에 등록된 상담사나 큐 간의 통화 횟수</td></tr><tr><td>내부 통화 시간</td><td>컨택 센터 내부에 등록된 상담사나 큐 간의 통화 시간</td></tr><tr><td>내부 통화 - %</td><td>컨택 센터 내부에 등록된 상담사나 큐 간의 통화 비율</td></tr><tr><td>내부 통화 - 평균</td><td>컨택 센터 내부에 등록된 상담사나 큐 간의 통화 평균 시간</td></tr><tr><td>협의 통화 횟수</td><td>상담사가 통화 중 다른 상담사와 협의를 위해 내선에서 다른 상담사나 외부 전화로 연결된 통화 횟수</td></tr><tr><td>협의 통화 시간</td><td>상담사가 통화 중 다른 상담사와 협의를 위해 내선에서 다른 상담사나 외부 전화로 연결된 통화 시간</td></tr><tr><td>협의 통화 - %</td><td>상담사가 통화 중 다른 상담사와 협의를 위해 내선에서 다른 상담사나 외부 전화로 연결된 통화 비율</td></tr><tr><td>협의 통화 - 평균</td><td>상담사가 통화 중 다른 상담사와 협의를 위해 내선에서 다른 상담사나 외부 전화로 연결된 통화 평균 시간</td></tr><tr><td>전환 통화 횟수</td><td>상담사나 큐로 부터 다른 상담사나 큐로 전환 연결된 통화 횟수</td></tr><tr><td>전환 통화 시간</td><td>상담사나 큐로 부터 다른 상담사나 큐로 전환 연결된 통화 시간</td></tr><tr><td>전환 통화 - %</td><td>상담사나 큐로 부터 다른 상담사나 큐로 전환 연결된 통화 비율</td></tr><tr><td>전환통화 - 평균</td><td>상담사나 큐로 부터 다른 상담사나 큐로 전환 연결된 통화 평균 시간</td></tr><tr><td>회의 통화 횟수</td><td>3명 이상의 다자간 통화 횟수. (흔히, 고객, 담당 상담사, 매니저 상담사의 3자 통화)</td></tr><tr><td>회의 통화 시간</td><td>3명 이상의 다자간 통화 시간. (흔히, 고객, 담당 상담사, 매니저 상담사의 3자 통화)</td></tr><tr><td>회의 통화 - %</td><td>3명 이상의 다자간 통화 비율. (흔히, 고객, 담당 상담사, 매니저 상담사의 3자 통화)</td></tr><tr><td>회의 통화 - 평균</td><td>3명 이상의 다자간 통화 평균 시간. (흔히, 고객, 담당 상담사, 매니저 상담사의 3자 통화)</td></tr><tr><td>직접 인입 횟수</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수의 횟수</td></tr><tr><td>직접 인입 시간</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수의 시간</td></tr><tr><td>직접 인입 - %</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수의 비율</td></tr><tr><td>직접 인입 - 평균</td><td>큐를 통하지 않고 전화기를 통해 상담사에게 들어온 호수의 평균 시간</td></tr></tbody></table>

### 상담 실적(점유)

상담사별 실적 (점유) 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%20%EC%8B%A4%EC%A0%81%20%EC%A0%90%EC%9C%A0.png" alt=""><figcaption><p>상담 실적 점유</p></figcaption></figure>

<table><thead><tr><th width="193">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 이름</td></tr><tr><td>상담사 ID</td><td>상담사 일련번호</td></tr><tr><td>상담사명</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 소속 그룹</td></tr><tr><td>팀</td><td>상담사 소속 팀</td></tr><tr><td>상담 채널</td><td>연결 미디어 타입</td></tr><tr><td>대기 - 대기 시간</td><td>대기 상태 유지된 시간</td></tr><tr><td>대기 - 대기 횟수</td><td>대기 상태로 변경된 횟수</td></tr><tr><td>처리 - 처리 시간</td><td>대기 상태의 상담원이 전화를 받거나 걸어서 통화한 시간</td></tr><tr><td>처리 - 처리 횟수</td><td>대기 상태의 상담원이 전화를 받거나 걸어서 통화한 횟수</td></tr><tr><td>후 처리 - 후처리 시간</td><td>후 처리 상태 유지된 시간</td></tr><tr><td>후 처리 - 후처리 횟수</td><td>후 처리 상태로 변경된 횟수</td></tr><tr><td>휴식 - 휴식 시간</td><td>휴식 상태 유지된 시간</td></tr><tr><td>휴식 - 휴식 횟수</td><td>휴식 상태로 변경된 횟수</td></tr></tbody></table>

### 상담 상태(총합)

상담사 상태를 총합으로 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%20%EC%83%81%ED%83%9C%20%EC%B4%9D%ED%95%A9.png" alt=""><figcaption><p>상담 상태 총합</p></figcaption></figure>

### 상담 사유(총합)

상담사 사유를 총합으로 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%20%EC%82%AC%EC%9C%A0%20%EC%B4%9D%ED%95%A9.png" alt=""><figcaption><p>상담 사유 총합</p></figcaption></figure>

<table><thead><tr><th width="138">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 이름</td></tr><tr><td>상담사 ID</td><td>상담사 일련번호</td></tr><tr><td>상담사명</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 소속 그룹</td></tr><tr><td>팀</td><td>상담사 소속 팀</td></tr><tr><td>옴니 채널</td><td>연결 미디어 타입</td></tr><tr><td>상태</td><td>현재 상담사 상태 (휴식, 후 처리, 로그아웃)<br> - 로그 오프 = { 0: 일반, 1: 식사, 2: 퇴근, 3: 조회, 4: 비번, 5: 휴가, 6: 외근, 7: 출장, 8: 지각, 9: 수리 }<br> - 휴식 = { 0: 일반, 1: 개인, 2: 식사, 3: 티타임, 4: 교육, 5: 회의, 6: 상담, 7: 다른 업무, 8: 개인업 무, 9: 수리 }<br> - 후처리 = { 1: 전산 처리, 2: 문서 처리, 3: 업무 처리, 4: 고객 상담, 5: 업무 지시, 6: 협의, 7: 외부 문의, 8: 다른 업무, 9: 수리 }</td></tr><tr><td>사유</td><td>상담원이 휴식, 후 처리, 로그 오프시 기록한 사유</td></tr><tr><td>시간</td><td>사유에 대한 시간</td></tr><tr><td>횟수</td><td>사유에 대한 횟수</td></tr></tbody></table>

### 상담 요약 현황

상담사별 요약 현황을 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%20%EC%9A%94%EC%95%BD%20%ED%98%84%ED%99%A9.png" alt=""><figcaption><p>상담 요약 현황</p></figcaption></figure>

<table><thead><tr><th width="179">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 이름</td></tr><tr><td>상담사 ID</td><td>상담사 일련번호</td></tr><tr><td>상담사명</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 소속 그룹</td></tr><tr><td>팀</td><td>상담사 소속 파트</td></tr><tr><td>상담 채널</td><td>연결 미디어 타입</td></tr><tr><td>I/B통화</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인바운드 통화 횟수</td></tr><tr><td>I/B통화 시간</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인바운드 통화 시간</td></tr><tr><td>I/B평균통화시간</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인바운드 통화 평균 시간</td></tr><tr><td>I/B통화 초 환산</td><td>고객으로부터 상담사에게 연결된 통화로서 PSTN을 통한 인바운드 통화 시간을 초로 환산</td></tr><tr><td>O/B접속</td><td>상담사으로부터 고객에게 연결 한 아웃바운드 접속 횟수</td></tr><tr><td>O/B통화</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃바운드 통화 횟수</td></tr><tr><td>O/B통화 시간</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃바운드 통화 시간</td></tr><tr><td>O/B평균 통화 시간</td><td>상담사로부터 고객에게 연결된 통화로서 PSTN을 통한 아웃바운드 통화 평균 시간</td></tr><tr><td>후 처리 시간</td><td>후 처리 상태 유지된 시간</td></tr><tr><td>후처리 횟수</td><td>후처리 상태로 변경된 횟수</td></tr><tr><td>대기 시간</td><td>대기 상태 유지 시간</td></tr><tr><td>대기 횟수</td><td>대기 상태로 변경된 횟수</td></tr><tr><td>평균 대기 시간</td><td>대기 시간 / 대기 건수</td></tr><tr><td>다른 업무</td><td>“휴식 - 다른 업무”로 변경된 총 시간</td></tr><tr><td>식사</td><td>“휴식 - 식사”로 변경된 총 시간</td></tr><tr><td>휴식</td><td>“휴식 - 휴식”으로 변경된 총 시간</td></tr></tbody></table>

### 상담사 일일 작업 현황

일별로 상담사의 작업 현황을 조회합니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%EC%82%AC%20%EC%9D%BC%EC%9D%BC%20%EC%9E%91%EC%97%85%20%ED%98%84%ED%99%A9.png" alt=""><figcaption><p>상담사 일일 작업 현황</p></figcaption></figure>

<table><thead><tr><th width="194">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 이름</td></tr><tr><td>상담사 ID</td><td>상담사 일련번호</td></tr><tr><td>상담사명</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 소속 그룹</td></tr><tr><td>팀</td><td>상담사 소속 팀</td></tr><tr><td>상담 채널</td><td>연결 미디어 타입</td></tr><tr><td>로그인 시간</td><td>상담사 로그인 시간</td></tr><tr><td>로그 아웃 시간</td><td>상담사 로그아웃 시간</td></tr><tr><td>대기 - 대기 시간</td><td>대기 상태 유지된 시간</td></tr><tr><td>대기 - 대기 횟수</td><td>대기 상태로 변경된 횟수</td></tr><tr><td>처리 - 처리 시간</td><td>대기 상태의 상담사가 전화를 받거나 걸어서 통화한 시간<br> - 인바운드는 상담사 전화기에 벨이 울리는 순간부터 아웃바운드 수화기를 든 순간부터 통화가 끝날 때까지의 시간</td></tr><tr><td>처리 - 처리 횟수</td><td>대기 상태의 상담사가 전화를 받거나 걸어서 통화한 횟수</td></tr><tr><td>후처리 - 후 처리 시간</td><td>후 처리 상태 유지된 시간</td></tr><tr><td>후처리 - 후 처리 횟수</td><td>후 처리 상태로 변경된 횟수</td></tr><tr><td>휴식 - 휴식 시간</td><td>휴식 상태 유지된 시간</td></tr><tr><td>휴식 - 휴식 횟수</td><td>휴식 상태로 변경된 횟수</td></tr><tr><td>인바운드 - 통화시간</td><td>상담사 인바운드 통화한 시간</td></tr><tr><td>인바운드 - I/B통화</td><td>상담사 인바운드 통화한 건수</td></tr><tr><td>아웃바운드 - 통화시간</td><td>상담사 아웃바운드 통화한 시간</td></tr><tr><td>아웃바운드 - O/B통화</td><td>상담사 아웃바운드 통화한 건수</td></tr></tbody></table>

### 상담사 로그인/로그아웃

상담사의 로그인/로그아웃 시간을 조회합니다. 1일 기준 상담사가 처음 로그인하여 로그아웃 할 때까지의 현황이 표현됩니다.

<figure><img src="https://t1.kakaocdn.net/service_kep_docpublish/Figma/KiCC/csapp/%EC%83%81%EB%8B%B4%EC%82%AC%20%EB%A1%9C%EA%B7%B8%EC%9D%B8%20%EB%A1%9C%EA%B7%B8%EC%95%84%EC%9B%83.png" alt=""><figcaption><p>상담사 로그인 로그아웃</p></figcaption></figure>

<table><thead><tr><th width="192">구분</th><th>설명</th></tr></thead><tbody><tr><td>테넌트</td><td>테넌트 이름</td></tr><tr><td>상담사 ID</td><td>상담사 일련번호</td></tr><tr><td>상담사명</td><td>상담사 이름</td></tr><tr><td>그룹</td><td>상담사 소속 그룹</td></tr><tr><td>팀</td><td>상담사 소속 팀</td></tr><tr><td>옴니 채널</td><td>연결 미디어 타입(Call or Chat)</td></tr><tr><td>로그 인 시간</td><td>상담사 로그인 시간</td></tr><tr><td>로그 아웃 시간</td><td>상담사 로그아웃 시간(null인 경우 로그인 상태)</td></tr><tr><td>등록 시간</td><td>상담사 로그인 유지 시간</td></tr></tbody></table>

