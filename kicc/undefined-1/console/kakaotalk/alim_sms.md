# 알림톡/SMS 연동 설정

## 사전 준비 사항 <a href="#prepare" id="prepare"></a>

* 연동 설정을 위해서 카카오톡 채널 관리자센터에서 본인 소유의 카카오톡 채널이 비즈니스 채널로 승인된 상태로 준비되어 있어야합니다.
* 카카오톡 채널 관리자 센터에서 아래 설정이 되어 있어야 정상적으로 연동/발송이 가능합니다.&#x20;
  * 프로필 > 프로필 설정 > **‘채널 공개’ ON**
  * 프로필 > 채널홈 설정 > 기본 정보 > **고객센터 전화번호 입력**&#x20;

{% hint style="info" %}
**사전 준비 사항 관련 링크**&#x20;

* [카카오톡 채널 관리자 센터 바로가기 ↗️](https://center-pf.kakao.com/)&#x20;
* [카카오 채널 & 비즈니스 채널 가이드 바로가기 ↗️](https://docs.kakaoi.ai/kakao_i_connect_message/bizmessage/#step-3-%EC%B9%B4%EC%B9%B4%EC%98%A4-%EC%B1%84%EB%84%90-%EC%83%9D%EC%84%B1-%EB%B0%8F-%EB%B9%84%EC%A6%88%EB%8B%88%EC%8A%A4-%EC%B1%84%EB%84%90-%EC%9D%B8%EC%A6%9D)&#x20;
* [[#sms](alim_sms.md#sms "mention") <mark style="color:blue;">가이드 바로가기 ↗️</mark>](https://kakaoenterprise.gitbook.io/kicc/guide/console/kakaotalk/alim_sms#sms)
{% endhint %}



## 연동 설정 하기

아래 화면에서 알림톡 및 SMS 연동을 진행합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (144).png" alt=""><figcaption><p>알림톡 및 SMS 연동</p></figcaption></figure>

### 알림톡 연동 설정 <a href="#alim-talk" id="alim-talk"></a>

기존에 다른 상담앱과 연동되어있는 알림톡 채널이어도 추가 연동 가능합니다. 사업자 카테고리는 카카오톡 채널 관리자센터에 등록된 카테고리와 유사한 카테고리로 선택해주시면 됩니다.

### SMS 연동 설정 <a href="#sms" id="sms"></a>

SMS 연동은 알림톡 발송 실패시 SMS 대체 발송 옵션을 사용하고자 할 경우 필요합니다.&#x20;

SMS 대체 발송이 진행되는 케이스는 아래와 같습니다.&#x20;

* 수신 고객이 카카오톡 앱을 사용하지 않을 경우
* 수신 고객이 해당 알림톡 채널을 '채널 차단 > 알림톡 차단'을 했을 경우
* 카카오톡 알림톡 발송 장애로 알림톡 발송이 실패했을 경우

SMS 발신번호 연동을 위해서는 통신사에서 발행한 통신서비스이용증명원 첨부가 필요하며, 증명원 상의 발신번호와 입력한 발신번호가 동일해야합니다. 등록 가능한 발신번호 세칙은 아래와 같습니다.

|                      | 세칙                                                  | 예시                                                                                                                               |
| -------------------- | --------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 공통                   | 실제 발신(통화)가 가능한 번호만 허용                               | <p>불가: 0000, 1004<br>가능: 1600-<strong>,</strong> 010--****</p>                                                                   |
| 일반 유선번호              | 일반 유선번호의 경우 17개 지역번호 (ex. 02, 031)를 앞자리에 포함한 번호만 허용 | <p>불가: 111-1111<br>가능: 02-111-1111</p>                                                                                           |
| 전국 대표번호, 공통서비스 식별 번호 | 지역번호 및 내선번호 포함 불가                                   | <p>불가: 02-1600-<em><strong>,</strong></em> 031-080<strong>-</strong>-***<br>가능: 1600-<em><strong>,</strong></em> 080-***-***</p> |
| 특수번호                 | 해당 사용자(국가, 공공기관)에 한해서만 사용 가능                        | 불가: 112, 1335                                                                                                                    |



## 알림톡/SMS 발송 <a href="#auto" id="auto"></a>

알림톡/SMS 연동 설정을 하면 아래의 기능을 사용할 수 있습니다.

{% hint style="info" %}
**알림톡/SMS 발송 기능 구분**

* 알림톡/SMS 자동 발송
  * 스마트 콜백 접수 알림톡
  * 상담사 상담 종료 알림톡
  * AI상담사 상담 종료 알림톡
* 상담앱에서의 알림톡/SMS 수동 발송&#x20;
{% endhint %}

센터플로우에서는 AI 컨택센터 운영 중 꼭 필요한 알림톡 4가지의 자동 발송 기능을 선택옵션으로 제공합니다. 모든 알림톡은 발송 실패시 SMS(LMS/MMS)로 대체 발송 가능하며 각 선택옵션별로 대체 발송 여부를 선택할 수 있습니다.



### 알림톡/SMS 자동 발송

#### 1️⃣ 스마트 콜백 접수 알림톡 <a href="#smart-callbaclk" id="smart-callbaclk"></a>

스마트 콜백은 AI 전화음성봇이 포함된 올인원 플랜을 사용할 경우 기본 제공되는 기능으로, 봇과의 대화 중 상담사 연결을 요청했으나 연결이 어려운 상황에서 봇이 상담사에게 나중에 전화를 다시 받을 수 있도록 콜백 접수를 하는 기능입니다. 콜백 접수가 정상적으로 완료되었을 경우, 접수 정보를 고객에게 알림톡으로 발송합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (105).png" alt=""><figcaption><p>스마트콜백 접수 알림톡</p></figcaption></figure>

#### 2️⃣ 상담사 상담 종료 알림톡 <a href="#counselor-chat-end" id="counselor-chat-end"></a>

플랜에 상관없이 사용할 수 있는 알림톡입니다. 고객과 상담사의 통화 종료 직후 알림톡을 발송합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (102).png" alt=""><figcaption><p>상담 종료 알림톡 (상담사)</p></figcaption></figure>

#### 3️⃣ AI 상담사 상담 종료 알림톡 <a href="#ai-chat-end" id="ai-chat-end"></a>

AI 전화 음성봇 사용시 적용할 수 있는 알림톡입니다. 고객과 AI 상담사의 통화 종료 직후 알림톡을 발송합니다.

<figure><img src="../../../.gitbook/assets/image (103).png" alt=""><figcaption><p>상담 종료 알림톡 (AI상담사)</p></figcaption></figure>

### 알림톡/SMS 수동 발송 <a href="#manual" id="manual"></a>

콘솔에서 알림톡/SMS 연동 설정시, 알림톡/SMS 수동 발송 기능을 사용할 수 있습니다.

{% hint style="info" %}
[상담앱 알림톡 수동 발송 가이드 보기 ↗️](https://guide.centerflow.kakaocloud.com/guide/counselling/counselor/sms#undefined)
{% endhint %}

{% hint style="info" %}
[상담앱 SMS 수동 발송 가이드 보기 ↗️](https://guide.centerflow.kakaocloud.com/guide/counselling/counselor/sms#sms-lms-mms)
{% endhint %}



## 발송 비용

알림톡/SMS 연동을 위한 추가 비용은 없으며, 사용량 기준으로 아래의 단가로 과금이 됩니다.&#x20;

<table><thead><tr><th width="126">구분</th><th>발송 단가</th></tr></thead><tbody><tr><td>알림톡</td><td>6원/건당</td></tr><tr><td>SMS</td><td>9원/건당</td></tr><tr><td>LMS</td><td>27원/건당</td></tr><tr><td>MMS</td><td>65원/건당</td></tr></tbody></table>
