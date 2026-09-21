# AI 봇 답변 설정 (스마트 알림톡/접수)

**서비스 관리 > AI 전화 음성봇 > AI 봇 답변 설정**에서는 나의 AI 전화 음성봇이 답변할 고객 문의 항목을 선택하고, 문의에 대한 AI의 답변을 입력할 수 있습니다. 필요 시 AI 답변과 함께 **스마트 알림톡**, **스마트 접수**와 같은 보조 기능을 설정하여 더욱 빠르고 효율적으로 상담을 처리하실 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

## 1. 고객 문의 유형 선택 <a href="#inquiry-type" id="inquiry-type"></a>

* **문의 유형이란:** 고객 문의 유형은 고객의 질문에서 동일한 의도를 가진 문장들의 묶음으로, 선택하신 업종별 봇 템플릿 기준으로 미리 머신러닝 학습되어 제공되는 질문들 입니다.&#x20;
* **문의 유형 선택:** 원하는 문의 유형을 선택하면, 해당 유형의 세부 문의 목록이 하단에 노출되어 원하는 세부 문의 항목을 선택하고 답변을 입력하면 됩니다.

{% hint style="info" %}
**업종별 봇 템플릿**

* 현재 홈페이지 구독하기를 통해서는 **이커머스** 업종 템플릿의 문의 유형만 제공되고 있지만, \
  그 외 **오프라인 소매점, 치과, 안과, 골프** 업종을 위한 봇 템플릿도 준비되어 있으니, \
  [**별도 문의**](https://centerflow.kakaocloud.com/support) 주시면 별도 설정을 통해 콘솔에서 확인 가능하십니다.
* 이커머스 봇템플릿에 대한 상세 내용은 [**여기**](https://guide.centerflow.kakaocloud.com/guide/console/ai_config/template)에서 확인해 주세요.
{% endhint %}



## 2. 문의에 대한 AI답변 입력 <a href="#ai-answer" id="ai-answer"></a>

선택한 문의 유형 하위의 세부 문의 항목을 선택하고, 선택한 세부 문의에 대한 답변을 입력하고, 필요 시 답변과 함께 발송할 알림톡 템플릿 정보 혹은 스마트 접수 설정 정보를 입력하여 나만의 봇을 완성합니다.&#x20;



### 1) 세부 질문 선택

* 선택한 문의 유형에 속한 세부 질문 중 나의 봇에서 필요한 질문을 탐색합니다.&#x20;
* 세부 문의 선택 시, 예시질문 우측의  \[↗️] 버튼을 클릭하여 예시 질문 목록을 참고하여 결정하시는 것을 권장 드립니다.&#x20;
*   예시 문 목록은 봇에 미리 학습되어 있는 문장 목록으로, 예시 질문과 관련성 높은 질문일 경우 봇이 잘 이해하고 인식하여 답변할 수 있습니다. <br>

    <figure><img src="../../../.gitbook/assets/image (37).png" alt="" width="563"><figcaption><p>예시 질문 목록</p></figcaption></figure>

### 2) 답변 입력

* 예시 질문 목록을 확인하고, 질문에 맞게 답변을 작성해 주세요.&#x20;
* \[예시 답변 불러오기] 체크박스를 클릭하시면, 권장 답변을 참고하여 작성하실 수도 있습니다. &#x20;
* 세부질문/답변 세트는 최소 5개를 입력해야 봇을 개통할 수 있습니다.
* 답변을 입력하고 최종적으로 하단의 \[저장/배포] 버튼을 클릭해야 실제 봇에 적용이 됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (173).png" alt=""><figcaption><p>답변 입력창</p></figcaption></figure>

### 3) 답변 수정/삭제 <a href="#modify-answer" id="modify-answer"></a>

&#x20;답변 수정이 필요한 경우, 콘솔에서 답변 수정 및 배포가 가능하며, 서비스 시작 전/후로 모두 가능합니다.&#x20;

* **답변 수정:** 답변을 수정 입력하고, 하단의 \[저장/배포] 버튼을 누르면 수정 사항이 즉시 봇에 반영됩니다.&#x20;
* **답변 삭제:** 우측 상단의 \[답변 초기화] 버튼을 클릭하고 \[확인] 버튼을 클릭하면 입력해둔 답변이 모두 사라지며, \[저장/배포] 클릭시 최종 반영 됩니다.&#x20;

{% hint style="info" %}
시작 요청 이후 단계로 회원 상태가 '테스트 가능', '이용 중' 상태라면, \
우측 상단의 **\[정보 수정]** 버튼을 클릭하셔야, 답변 수정이 가능합니다.&#x20;
{% endhint %}



## 3. 스마트 알림톡 설정

### 1) 스마트 알림톡 시나리오

{% hint style="info" %}
**스마트 알림톡이란?**

* 상담봇의 음성 안내만으로는 답변이 충분하지 않을 경우, 간단한 봇 답변과 함께 카카오톡 알림톡을 발송할 수 있습니다.&#x20;
* 알림톡에 상세 설명과 함께 웹사이트, 영상 등의 자료 링크를 추가하면 좀더 완결성 있는 안내가 가능하며,  재문의도 줄일 수 있습니다.&#x20;
{% endhint %}

<div align="left"><figure><img src="../../../.gitbook/assets/image (177).png" alt=""><figcaption><p>스마트알림톡 동작 방식</p></figcaption></figure></div>

### 2) 알림톡 정보 입력

*   **Step1. 세부 문의 별 \[스마트 알림톡 설정하기] 버튼 클릭**

    * **'AI 전화 음성봇 > 봇 답변 설정'** 메뉴의 세부 문의 리스트에서 스마트 알림톡을 설정하고자 하는 세부문의를 선택하여 답변 입력창을 열고, **\[스마트 알림톡]** 버튼을 클릭하면 세부 정보 설정 팝업이 노출 됩니다.&#x20;
    * [**알림톡/SMS 연동 설정**](../kakaotalk/alim_sms.md) 메뉴에서 카카오톡 비즈니스 채널에 등록 완료된 상태여야, 스마트 알림톡 설정 팝업에 진입할 수 있습니다. <br>

    <figure><img src="../../../.gitbook/assets/image (174).png" alt=""><figcaption><p>스마트알림톡 버튼</p></figcaption></figure>


* **Step2. 알림톡 템플릿 코드 입력**
  * 스마트 알림톡 팝업에서 봇 답변과 함께 발송하고자 하는 알림톡 템플릿의 코드를 입력합니다.&#x20;
  * 비즈메시지 어드민에서 등록/검수요청 후 '승인' 상태인 템플릿 코드를 입력해야, \[코드 확인] 클릭 시 정상 등록이 가능합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (26).png" alt=""><figcaption><p>스마트 알림톡 설정 팝업</p></figcaption></figure>

{% hint style="info" %}
[**비즈메시지 어드민 바로가기 ↗️**](https://bizmsg-web.kakaoenterprise.com/user/login)

* 비즈메시지 어드민에서 발송하고자 하는 우리 회사만의 알림톡 템플릿을 등록 후, 검수/승인의 과정을 거칩니다 (1\~2 영업일 소요)
* 비즈메시지 어드민의 ID/PW와 가이드는 센터플로우 콘솔에서 [카카오톡 알림톡 연동 설정](https://kakaoenterprise.gitbook.io/kicc/guide/console/kakaotalk/alim_sms)을 한 고객사에 한하여, 서비스 개통일 이전에 별도 이메일로 안내됩니다.&#x20;
{% endhint %}

* **Step3. SMS 대체발송 설정**
  * 알림톡/SMS 연동 설정 메뉴에서 대체 발송 번호를 등록 완료한 상태여아, 스마트 알림톡 팝업에서 SMS 대체 발송 설정을 할 수 있습니다.&#x20;
  *   대체 발송이 진행되는 케이스는 아래 가이드를 참고해 주세요.&#x20;

      &#x20;👉 [SMS 대체 발송 케이스](https://kakaoenterprise.gitbook.io/kicc/guide/console/kakaotalk/alim_sms#sms)

{% hint style="info" %}
**안내**

* 스마트 알림톡 설정시 봇의 답변과 함께 알림톡 메시지를 발송한 뒤 통화를 자동 종료하는 것을 기본 시나리오로 하며, 권장합니다. 통화를 종료하지 않고 다른 문의를 이어 받고자 할 경우, 별도 문의해 주세요.
* 알림톡/SMS/LMS 발송 요금은 아래 가이드를 참고해주세요\
  &#x20;👉 [발송 요금 안내](https://kakaoenterprise.gitbook.io/kicc/guide/console/kakaotalk/alim_sms#undefined-1)
{% endhint %}



### 3) 스마트 알림톡용 봇 답변 입력

* 스마트 알림톡 팝업에서 설정 완료 시, 아래와 같이 봇 답변 입력창이 변경됩니다.&#x20;
* 스마트 알림톡을 발송하는 '세부 문의'일 경우, 콘솔에 입력한 봇의 답변에 바로 뒤이어, 알림톡 수령 여부를 고객에게 질의하기 때문에, "카카오톡으로 상세 정보를 전송해드리겠습니다. 지금 거신 번호로 보내드릴까요?"라는 문장이 이어질 때 자연스러운 답변으로 입력해주세요.

<figure><img src="../../../.gitbook/assets/image (175).png" alt=""><figcaption><p>스마트 알림톡용 답변 입력 예시</p></figcaption></figure>



### 4) 스마트 알림톡 설정 수정/삭제

* **알림톡 설정 수정:** 한번 설정 완료한 스마트 알림톡은 'SMS 대체 발송 사용'과 '대체 발송 문구'만 수정이 가능하며, 템플릿 코드를 수정하고자 할 경우에는 \[삭제] 후 재입력하셔야 합니다.&#x20;
* **알림톡 설정 삭제:** 아래 팝업에서 \[삭제] 버튼을 클릭하여 봇에 즉시 반영 가능합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (26).png" alt=""><figcaption><p>알림톡 설정 완료 후 팝업</p></figcaption></figure>



## 4. 스마트 접수 설정 <a href="#add-modify" id="add-modify"></a>

{% hint style="warning" %}
<mark style="color:red;">스마트접수는 콘솔에서 세부 문의 항목별로 설정할 수 있지만, 최초 설정시에 한해 별도 작업이 필요합니다.</mark> \ <mark style="color:red;">👉</mark> [별도 요청](https://pages.kakaoenterprise.com/connectcenter_support.html) 주시면 콘솔에서 입력하신 내용이 즉시 상용 봇에 적용되도록 설정 가능합니다.&#x20;
{% endhint %}

### 1) 스마트 접수 시나리오

{% hint style="info" %}
**스마트 접수란?**

* 상담봇이 처리할 수 없는 복잡한 문의사항이거나 강성/민감 문의일 경우, 상담봇이 응대하는 것보다 빠른 상담사 연결이 서비스에 도움이 됩니다. 스마트 접수는 상담사 연결이 필요한 문의를 봇이 분류하여 상담사에게 바로 연결합니다.
* 특정 문의에 대한 전문 상담사가 있다면, 봇의 세부 문의 항목별로 내선 지정하여 연결도 가능합니다. 설정을 원하시면 [별도 요청](https://centerflow.kakaocloud.com/support) 주세요.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

### 2) 스마트 접수 설정

**Step 1. 세부 문의별 \[스마트 접수 설정하기] 버튼 클릭**

<figure><img src="../../../.gitbook/assets/image (182).png" alt=""><figcaption></figcaption></figure>

**Step 2. 상세 내용 설정**

관리자 알림톡 전송 여부와 전송 받을 관리자 핸드폰 번호를 입력합니다. \
알림톡 비용은 건당 청구됩니다. ([알림톡 비용 참고](https://guide.centerflow.kakaocloud.com/guide/console/kakaotalk/alim_sms#undefined-1))

<figure><img src="../../../.gitbook/assets/image (179).png" alt=""><figcaption></figcaption></figure>

### 3) 스마트 접수용 봇 답변 입력 <a href="#add-modify" id="add-modify"></a>

스마트 접수를 설정하시면, 봇 답변 입력창이 아래와 같이 변경됩니다.&#x20;

* **근무 시간용 답변:** 근무시간에만 상담사에게 연결되는 것을 감안하여, 그리고 이어서 출력될 고정 답변의 문구와 잘 어울리도록 나만의 답변을 입력합니다.&#x20;
* **근무 외 시간용 답변:** 근무 외 시간에는 상담사 연결하지 않고, 상담앱에 스마트 접수를 등록하여, 상담사가 근무시간에 확인 후 콜백 할 수 있도록 합니다. 이어서 출력될 근무 외 시간용 고장 답변의 문구와 잘 어울리도록 나만의 답변을 입력합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (181).png" alt=""><figcaption></figcaption></figure>

### 4) 스마트 접수 설정 수정/삭제 <a href="#add-modify" id="add-modify"></a>

* **스마트 접수 수정:** 관리자 알림톡 설정 정보는 언제든 \[수정하기] 버튼을 눌러 변경이 가능하며, 봇 답변도 '봇 답변 설정' 메뉴에서 수정하실 수 있습니다.&#x20;
* **스마트 접수 삭제:** 스마트 접수 설정을 삭제하시려면 \[수정하기] 버튼을 클릭하여, '스마트 접수 설정' 토글 버튼을 OFF하시면 됩니다.&#x20;



## 4. 문의 유형 추가/변경 요청 <a href="#add-modify" id="add-modify"></a>

<figure><img src="../../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

* 봇 템플릿에서 제공되는 문의 유형 외에 다른 유형의 추가나 변경을 원할 경우 요청서를 제출할 수 있습니다.&#x20;
* 요청서를 제출하시면 '문의 유형 추가/변경 요청' 카드가 **'**<mark style="color:blue;">**처리중**</mark>**'** 상태로 변경됩니다.&#x20;
* 접수된 요청 사항은 담당자가 확인 후 논의를 거쳐 '맞춤 유형'으로 추가되어 콘솔에서 선택할 수 있게 됩니다.



<figure><img src="../../../.gitbook/assets/image (32).png" alt="" width="563"><figcaption><p>문의 유형 추가 요청 예시</p></figcaption></figure>

{% hint style="info" %}
**안내**

* 요청서를 접수하시면 담당자가 별도 연락을 드려, 요구사항을 상세 취합하고 상담봇이 해당 질문을 처리하는데 문제가 없을지 검토를 진행합니다.&#x20;
* 최종적으로 맞춤 유형 추가 시, 별도 비용이 발생될 수 있으며 이 또한 논의를 통해 확정합니다.&#x20;
{% endhint %}

{% hint style="success" %}
**참고**

* 단순 문의이면서 질문의 '키워드'가 명확한 경우, **키워드별 답변 설정** 메뉴에서 키워드와 답변을 직접 등록하시는 것으로 추가 비용 없이 간편하게 새로운 문의 유형에 대응하실 수 있습니다. \
  **👉** [**키워드별 답변 설정 가이드**](recommended.md)
{% endhint %}



## 5. 봇 응답 시 원하는 대로 TTS하기 (SSML태그 작성) <a href="#ssml" id="ssml"></a>

AI 전화 음성봇의 답변 작성 시, 의도대로 음성 합성되지 않는 텍스트는 'SSML 태그'를 사용하여 입력하면 원하는 대로 봇이 읽게 할 수 있습니다.&#x20;

### SSML 태그란?&#x20;

SSML (Speech Synthesis Markup Language, 음성 합성 마크업 언어) 은 TTS에 입력된 텍스트를 합성 음성으로 변환하는 방법을 지정할 수 있는 XML 기반의 마크업(Markup) 언어입니다. SSML 태그를 입력하면 음성봇이 TTS (Text-to-Speech)할 때 입력한 규칙대로 발음하게 됩니다. <br>

### 자주 사용하는 SSML 태그

#### **\<speak> 태그**<mark style="color:red;">**\***</mark>

음성으로 변환할 텍스트를 나타내는 **필수/기본 태그**입니다. 모든 텍스트는 반드시 태그 안에 작성되어야 합니다. SSML의 루트 요소이며, 태그를 제외한 모든 태그는 태그의 하위 요소로 존재할 수 있습니다.

태그는 문장, 문단 단위로 적용하는 것을 원칙으로 합니다. 만일 단어의 연속적인 나열을 합성하고자 할 경우, 음성 합성 품질을 위해 쉼표 등의 구두점으로 요소를 구분할 것을 권장합니다.

*   예시.&#x20;

    <pre class="language-jsx"><code class="lang-jsx"><strong>&#x3C;speak> 안녕하세요. 반가워요 &#x3C;/speak>
    </strong></code></pre>



#### **\<say-as> 태그**&#x20;

날짜, 시간과 같은 축약형 표현이나 전화번호, 스펠링의 발음 규칙을 상황에 맞게 커스텀 적용합니다. 입력한 속성값에 따라 모델이 특수 표현을 해석하여 음성을 합성합니다. `format` 속성은 `interpret-as` 속성의 속성값으로 `date`, `time`, `kakao:number`를 입력했을 때에만 함께 쓰입니다.

<table><thead><tr><th width="233">속성</th><th>속성값</th></tr></thead><tbody><tr><td><code>interpret-as</code></td><td><strong>단일 속성으로 사용 가능</strong><br>- <code>spell-out</code>: 영어 단어를 개별 알파벳으로 발음<br>- <code>digits</code>: 숫자를 하나씩 발음 (ex. 일, 이, 삼)<br>- <code>kakao:serial</code>: 숫자를 하나씩 읽되, -를 ‘다시’로 발음<br>- <code>telephone</code>: 전화번호 읽기처럼 0을 ‘공’으로, -를 ‘에’로 발음<br>- <code>kakao:none</code>: 원문을 적절한 조사로 적용하여 발음<br>- <code>kakao:score</code>: 스코어로 발음 (ex. 3:1 → 삼 대 일)<br>- <code>kakao:vocative</code>: 호격 조사를 적절하게 반영해 발음 (ex. 영숙야 → 영숙아)<br><br><strong>format 속성 필수 지정</strong><br>- <code>date</code>: 날짜 형식으로 발음<br>- <code>time</code>: 시간으로 발음<br>- <code>kakao:number</code>: 숫자의 고유어 또는 한자어 발음 선택</td></tr><tr><td><code>format date</code></td><td><strong>날짜 형식을 다양하게 조합 가능</strong> (ex. dmy, my, ymd, d, m 등)<br>- <code>y</code>: 년, <code>m</code>: 월, <code>d</code>: 일<br>- 조합된 순서대로 숫자를 대입해 발음<br>- <code>&#x3C;say-as></code> 태그를 적용할 날짜 표기법은 <code>-</code>, <code>/</code>, <code>.</code> 중 사용</td></tr><tr><td><code>format time</code></td><td><strong>시간 형식을 다양하게 조합 가능</strong> (ex. hms12, hm24, ms, hm, s 등)<br>- <code>h</code>: 시, <code>m</code>: 분, <code>s</code>: 초, <code>12</code>: 12시간제, <code>24</code>: 24시간제<br>- 조합된 순서대로 숫자를 대입해 발음<br>- 시간제 미입력 시, 오전/오후 없이 12시간제로 발음<br>- <code>&#x3C;say-as></code> 태그를 적용할 시간 표기법은 <code>:</code> 만 사용</td></tr><tr><td><code>format kakao:number</code></td><td><strong>숫자 읽기 방식 지정</strong><br>- <code>korean</code>: 숫자 고유어 발음 (ex. 한/하나, 두/둘, 세/셋)<br>- <code>chinese</code>: 숫자 한자어 발음 (ex. 일, 이, 삼)<br>- 수량 단위 명사를 <code>&#x3C;say-as></code> 태그 내에 작성</td></tr></tbody></table>

*   예시1. say-as 태그에 interpret-as 단일 속성 사용

    ```jsx
    <speak>
      <say-as interpret-as="spell-out">kakao</say-as>를 스펠링으로 읽어줍니다.
      <say-as interpret-as="digits">1987</say-as>, 숫자를 낱개로 읽어줍니다.
      <say-as interpret-as="telephone">82-010-1234-5678</say-as>, 휴대폰 번호를 잘 읽어줍니다.
      <say-as interpret-as="kakao:none">부처님 오신 날</say-as>가, 조사 처리도 잘해줍니다.
      <say-as interpret-as="kakao:score">3:1</say-as>로 이겼습니다. 스코어로 인식하고 읽어줍니다.
      <say-as interpret-as="kakao:vocative">영숙</say-as>야.
      <say-as interpret-as="kakao:vocative">톤</say-as>야.
    </speak>
    ```

    🎧 [음원 듣기](https://objectstorage.kr-central-1.kakaocloud.com/v1/797c9fa126ea4678b2137074647faa18/general-tts-guide/ssml/say-as-1.mp3)<br>
*   예시2. \<say-as> 태그에 format 필수 속성 사용

    ```jsx
    <speak>
      <say-as interpret-as="date" format="dmy">10.6.85</say-as> 입니다.
      <say-as interpret-as="date" format="my">10.1985</say-as> 입니다.
      <say-as interpret-as="date" format="md">10-6</say-as> 입니다.
      <say-as interpret-as="date" format="d">10</say-as> 입니다.
      <say-as interpret-as="time" format="hms12">13:16:45</say-as> 입니다.
      <say-as interpret-as="time" format="hm24">13:50</say-as> 입니다.
      <say-as interpret-as="time" format="ms">10:59</say-as> 입니다.
      <say-as interpret-as="time" format="h">13</say-as> 입니다.
      <say-as interpret-as="kakao:number" format="chinese">13장</say-as> 입니다.
      <say-as interpret-as="kakao:number" format="korean">13장</say-as> 입니다.
    </speak>
    ```

    🎧 [음원 듣기](https://objectstorage.kr-central-1.kakaocloud.com/v1/797c9fa126ea4678b2137074647faa18/general-tts-guide/ssml/say-as-2.mp3)<br>

#### **\<sub> 태그**

특정 단어의 발음을 직접 지정합니다. 자사의 상호/브랜드명과 같이 특정한 규칙에 따라 읽어야하는 경우에 적용할 수 있습니다. 속성값은 모델의 해석이 용이하도록 한글로 작성합니다.

<br>

| 속성    | 속성값                                                                  |
| ----- | -------------------------------------------------------------------- |
| alias | <p></p><p>합성 요청 텍스트 대신 발음할 단어를 직접 입력</p><ul><li>가능한 한글로 입력</li></ul> |

*   예시

    ```
    <speak><sub alias="알루미늄">Al</sub>은 단단하다.</speak>
    ```

    🎧 [음원 듣기](https://objectstorage.kr-central-1.kakaocloud.com/v1/797c9fa126ea4678b2137074647faa18/general-tts-guide/ssml/sub.mp3)



{% hint style="info" %}
**그 외 태그 적용 안내** \
위의 SSML 태그 외에 아래와 같은 다른 태그의 사용을 희망할 경우 [별도 문의](https://centerflow.kakaocloud.com/support) 바랍니다. \
요구사항 확인 후 지원해드릴 수 있도록 하겠습니다.&#x20;

* voice (목소리)
* prosody (읽기 속도/크기)
* break (끊어읽기)
* audio (외부 음원 파일 재생)
{% endhint %}



### 특수 문자 코드에 대한 TTS 기본 규칙

SSML태그를 적용하지 않아도, 기본적인 문자코드들은 모두 정규화 규칙에 따라 자동으로 TTS 처리되어 읽어주고 있습니다. 지원하는 문자 코드에는 영문 알파벳, 한글 음절 및 자모, 숫자 및 숫자 포함 문자열, 이메일 및 URL, 기호, 문장 부호가 있으며, 상세한 처리 방식은 아래 내용을 참고해 주세요.&#x20;

| 항목             | 설명                                                                                                                                                                                                     | 예시                                                                                                                                                                                        |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 영문 알파벳         | 개별 알파벳 처리 가능                                                                                                                                                                                           | <p>a → 에이 <br>b → 비</p>                                                                                                                                                                   |
| 한글 음절 및 자모     | <p></p><p>음절(초성과 중성, 혹은 초성, 중성과 종성으로 구성된 단위) 처리를 원칙으로 함</p><ul><li>자모 낱자는 이름으로 읽음</li><li>자주 쓰이는 일부 초성 문자는 예외적으로 처리하여 읽음 ㄴ ex. ㅎㅎ, ㅋㅋ, ㅇㅋ, ㄴㄴ, ㅃㅇ, ㅎㅇ</li></ul>                                        | <p>ㄱ → 기역 </p><p>ㅏ → 아 </p><p>ㄷㄷ → 디귿디귿 </p><p>ㅋㅋ → 크크</p>                                                                                                                                |
| 한국어 한자         | <p></p><p>한국에서 쓰이는 한자</p><ul><li>중국, 일본에서 사용하는 간체는 처리하지 않음</li><li>음성 합성 엔진이 Deep Voice일 경우만 지원</li></ul>                                                                                              | <p>漢字는 外國 文字인가? → 한자는</p><p>외국 문자인가? </p><p>前 韓國外交協會 會長 → 전 한국외교협회 회장 </p><p>韓國漢詩協會 理事長 → 한국한시협회 이사장 </p><p>本聯合會 顧問 → 본연합회 고문</p>                                                         |
| 숫자 및 숫자 포함 문자열 | <p></p><p>숫자 읽기 처리</p><ul><li>전화번호로 판단되는 형식: 전화번호로 읽음</li><li>날짜 혹은 시간으로 판단되는 형식: 날짜 또는 시간으로 읽음</li><li>도량형 표기로 판단되는 형식: 도량형 단위로 읽음</li><li>영어 뒤에 오는 숫자는 영어로, 한글 뒤에 오는 숫자는 한글로 읽음</li></ul>            | <p>1987 → 천구백팔십칠 </p><p>02-1234-5678 → 공이에 일이삼사에 오육칠팔 </p><p>2017/7/5 → 이천십칠년 칠월 오일 </p><p>a.m. 7시 → 오전 일곱시 </p><p>10cm → 십센티미터 </p><p>100Hz → 백헤르쯔 </p><p>시즌1 → 시즌원 </p><p>안녕1 → 안녕일</p> |
| 이메일 및 URL      | <p></p><p>이메일이나 URL 형식의 문자열</p><ul><li>각각 “이메일 주소” 혹은 “링크”로 치환하여 읽음</li></ul>                                                                                                                          | <p><a href="mailto:cx@kakaoenterprie.com">cx@kakaoenterprie.com</a> → 이메일 주소<br><a href="https://kakaocloud.com">https://kakaocloud.com</a> → 링크</p>                                      |
| 기호             | <ul><li>Printable ASCII 코드에 포함된 특수기호: 문맥에 따라 읽거나 읽지 않음</li><li>UTF-8 유니코드 중 자주 쓰이는 도량형 기호를 읽어줌</li><li>괄호 내부 문자는 일반적으로 읽지 않으나, 뉴스 바이라인 형식으로 판단하는 경우 괄호 내 문자를 읽어줌</li></ul>                             | <p>100% → 백퍼센트 </p><p>$100 → 백달러 </p><p>100㎛ → 백마이크로미터</p>                                                                                                                                |
| 문장 부호          | <p>쉼표(,), 마침표(.), 느낌표(!), 물음표(?), 아포스트로피(’), 큰따옴표(”), 작은따옴표(’), 하이픈(-) 처리</p><p><br>•  <code>,</code> : 문장 내 끊어 읽기<br>•  <code>-</code> <code>.</code>, <code>?</code>, <code>!</code> : 억양과 길이 조절</p> |                                                                                                                                                                                           |

