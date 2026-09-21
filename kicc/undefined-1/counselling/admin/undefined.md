# 녹취 관리 시스템

## 녹취 관리 시스템

상담 애플리케이션 어드민에서 녹취 파일을 관리하는 녹취 관리 시스템 서버의 관리자 페이지로 이동하여 로그인할 수 있습니다. Admin 계정은 따로 로그인 없이 바로 접속이 가능합니다.<br>

<figure><img src="../../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

## 녹취 내역 관리

### 녹취 내역 관리

저장된 녹취 파일을 조회 , 청취, 다운로드할 수 있으며 녹취 파일 삭제는 불가합니다.

<figure><img src="../../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

#### 조회 조건

조회 조건을 설정하고 조회를 누르면 조건에 해당하는 녹취 파일의 목록이 노출됩니다.

| 구분      | 상세 설명                                                              |
| ------- | ------------------------------------------------------------------ |
| 회사      | 테넌트 이름                                                             |
| 통화종류    | IN : INBOUND 호                                                     |
|         | OUT : OUTBOUND 호                                                   |
| 상담원     | 상담사 ID                                                             |
| 이름      | 상담사 이름                                                             |
| 시작시간    | 녹취 시작 시각                                                           |
| 종료시간    | 녹취 종료 시각                                                           |
| 내선번호    | 상담사 내선번호(DN)                                                       |
| 연결번호    | 상담 고객 전화번호                                                         |
| 통화종료 번호 | 먼저 통화 종료를 시도한 번호 ( 내선번호 or 연결번호 중에 1개임 )                           |
| 통화시간(초) | 상담사와 고객 간 실제 통화를 한 시간 ( 녹취 파일 생성 옵션에 따라서 통화시간과 녹취파일 생성시간이 다를 수 있음) |
| 녹취 타입   | 전수 녹취                                                              |



#### 녹취 파일 원본 증명

최초 생성된 녹취 파일과 상담 애플리케이션 어드민을 통해서 다운받은 녹취 파일에 대해서 동일한 파일임을 확인할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>



\[파일 선택]을 클릭하여 기존에 다운받은 녹취 파일을 선택합니다.

선택 파일 해시와 서버 파일 해시가 동일하다면 녹취 파일이 원본이라는 것을 증명할 수 있습니다.

#### 녹취 파일 다운로드

녹취 파일을 선택하여 여러개 다운로드 하거나 개별로 다운로드 가능합니다.

<figure><img src="../../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>

다운로드 시에는 사유를 입력해야 합니다.

<figure><img src="../../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

#### 녹취 파일 재생

녹취 관리 시스템에서 저장된 녹취 파일을 직접 청취 가능합니다.

<figure><img src="../../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

## 콜 모니터링

### 콜 모니터링

상담 애플리케이션의 모든 콜에 대한 모니터링 기능을 제공하고 청취 기능을 제공합니다.

<figure><img src="../../../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

#### 조건

조건을 선택한 뒤 시작 버튼을 누릅니다.

<figure><img src="../../../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

현재 통화 중인 목록이 노출되며, AI 상담봇, 상담사와 통화 시 청취가 가능합니다.

<figure><img src="../../../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

## 녹취 사용량

### 녹취 사용량

상담사 내선번호별로 녹취 파일 사용량(녹취 파일 건수)를 조회합니다.

큐 대기 중에 종료된 호의 경우 상담사와 통화 연결이 되지 않았기 때문에 조회 대상에서 제외됩니다.

<figure><img src="../../../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

#### 녹취 목록

| 구분        | 상세 설명                                                        |
| --------- | ------------------------------------------------------------ |
| 내선번호      | 상담원 내선번호                                                     |
| 연결번호      | 상담 고객측 전화번호(착발신 구분없음)                                        |
| 날짜        | 녹취 파일이 생성된 날짜                                                |
| 레코드 개수    | 상담원 내선로 통화 연결되어 녹취파일이 생성 된 갯수 ( 해당 내선으로 착신된 INBOUND 호수와 동일함) |
| 총 통화시간(초) | 상담원 내선으로 통화 연결된 총 통화 시간                                      |

## 녹취 사용량 통계

### 녹취 사용량 통계

상담사 내선번호 기준으로 INBOUND , OUTBOUND 호를 구분하고 통화시간을 통계로 제공합니다.



## 로그인 이력

<figure><img src="../../../.gitbook/assets/스크린샷 2023-08-24 오전 10.00.19 (1).png" alt=""><figcaption></figcaption></figure>

#### 로그인 이력

녹취 관리 시스템으로 로그인한 이력을 제공합니다.

### 녹취 관리 이력

녹취 관리 시스템으로 접속하여 관리자가 실행한 모든 명령어에 대한 이력을 조회합니다.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a38193d7-040b-4722-9732-c9823fc2fab7/Untitled.png)

