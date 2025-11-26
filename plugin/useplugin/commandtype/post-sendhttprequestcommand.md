# Post 데이터 명령(SendHTTPRequestCommand)

타사 데이터 연결을 완료하기 위해 SendHTTPRequestCommand 플러그인을 사용합니다.&#x20;

일반적으로 타사에서 데이터 연결을 위한 API 문서를 아래와 같이 제공합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (507).png" alt=""><figcaption></figcaption></figure>

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/SendHTTPRequestCommand.zip">SendHTTPRequestCommand.zip</a></td></tr><tr><td>v 9.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/SendHTTPRequestCommand.zip">SendHTTPRequestCommand.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/SendHTTPRequestCommand.zip">SendHTTPRequestCommand.zip</a></td></tr><tr><td>v 7. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7_Plugin_20210722/SendHTTPRequestCommand.zip">SendHTTPRequestCommand.zip</a></td></tr><tr><td>v 6. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6.1_Plugin_20201111/SendHTTPRequestCommand.zip">SendHTTPRequestCommand.zip</a></td></tr></tbody></table>

### 사용방법&#x20;

1. 플러그인을 다운로드합니다.
2. Forguncy Builder에서 설치하고 Forguncy Builder를 다시 실행합니다.
3. 명령창에서 "POST 데이터 명령"을 선택하고 아래와 같이 설정합니다.&#x20;

{% hint style="info" %}
일반명령과 서버단 명령에서 사용할 수 있습니다.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (1230).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="183">항목 </th><th>설명 </th></tr></thead><tbody><tr><td>URL</td><td>사용자는 요청을 보낼 대상 URL을 지정해야 합니다. url 사용자 입력 또는 계산 결과가 ' http://' 로 시작하지 않고 ' https://' 로 시작하지 않는 경우 현재 웹사이트 기본 URL을 연결합니다.</td></tr><tr><td>Method</td><td>Http 메서드(GET,POST,PUT,DELETE)                                                            - GET / DELETE : 매개변수는 URL의 문자열에 있습니다.                             - POST/PUT: 매개변수는 요청의 본문의 내용입니다.  JSON 직렬화가 선택되지 않은 경우, 컨텐츠 유형은  <strong>application</strong> /x-www- <strong>form</strong> - <strong>urlencoded</strong> '이고, 그렇지 않으면 콘텐츠 유형은 'application/json'이 됩니다.</td></tr><tr><td>데이터유형 </td><td><ol><li>값 혹은 공식 : 데이터를 원격 서버로 보낼 단순 값(키 값 쌍 없음)임을 의미합니다.</li><li>복합구조 : 서버로 보내는 데이터에 어떤 속성이 있음을 의미합니다.</li><li>정렬 : 원격 서버에 값의 배열을 보낼 것임을 의미합니다.</li></ol><p>        - 자동: 디자이너에서 디자인한 개수와 동일한 포스트 데이터 배열                         </p><p>           개수를 의미합니다.</p><p>        - 지정된 수: 데이터 배열 개수가 지정되었음을 의미합니다. </p><p>           일반적으로 페이지의 상수 또는 공식(목록 보기 횟수)입니다. </p><p>4. 리스트뷰데이터 : 포건시 리스트뷰에서 데이터를 사용합니다. 리스트이름과 열이름이 필요합니다. </p></td></tr><tr><td>Json직렬화 </td><td>값이 json 문자열로 직렬화되는지 여부를 의미합니다. </td></tr><tr><td>POST 성공콜백</td><td>POST 성공 후 실행할 자바스크립트 코드. 결과 데이터는 ' result ' 변수에 저장됩니다.</td></tr><tr><td>POST 오류콜백</td><td>POST 실패 후 실행할 자바스크립트 코드. 오류 정보는 ' <strong>error</strong> ' 변수에 저장됩니다.</td></tr></tbody></table>

3-1. 일반적으로 데이터 양식을 아래와 같이 입력합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (615).png" alt=""><figcaption></figcaption></figure>

3-2. JSON 직렬화에 체크를 하면 Content Type이 "application/json; charset=UTF-8"인 것을 확인할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1655).png" alt=""><figcaption></figcaption></figure>

3-3. 복합구조의 값을 복합구조로 사용하려면 아래와 같이 사용할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1782).png" alt=""><figcaption></figcaption></figure>

3-4. 원격 API에 Json 배열을 게시하는 경우 아래와 같 사용할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1755).png" alt=""><figcaption></figcaption></figure>

3-5. 리스트뷰를 아래와 같이 사용할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1123).png" alt=""><figcaption></figcaption></figure>

리스트뷰 데이터의 모든 행을 가져와야 할 경우 아래와 같이 적용합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1636).png" alt=""><figcaption></figcaption></figure>

4\. 요청 결과를 셀 값으로 설정 할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1995).png" alt=""><figcaption></figcaption></figure>

요청 반환이 json인 경우 "**,**"속성을 이용하여 값을 얻을 수 있습니다.&#x20;

{% hint style="info" %}
반환 데이터값은 단순 값 또는 Json 형식이어야 합니다.

XML형식은 지원되지 않습니다.
{% endhint %}

예를 들어:

반환 데이터가 _{ Name: 'Jobs Smith', Age: 52, Sex: 'Male', Company:  { Name: 'Apple', Location: 'USA' } }_ 이고 새 매개변수가 'result'인 경우, "**result.Comapny.Location**" 으로 json 내부 속성 값을 가져옵니다.&#x20;

### 서버단 명령 지원&#x20;

사용자가 서버에서 요청을 보내야하는 경우가 있습니다. 브라우저에서 요청하면 교차 도메인 문제가 발생할 수 있기 때문입니다. 사용법은 일반 명령과 거의 동일하지만 몇 가지 차이점이 있습니다.&#x20;

1.서버 단 명에서 리스트뷰 데이터를 지원하지 않습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1721).png" alt=""><figcaption></figcaption></figure>

2\. 결과는 파라미에 의해 나옵니다. 다른 명령에서 해당 파라미터를 사용할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1751).png" alt=""><figcaption></figcaption></figure>

요청 반환이 json인 경우 ","속성을 이용하여 값을 얻을 수 있습니다.&#x20;



예를 들어:

반환 데이터가 _{ Name: 'Jobs Smith', Age: 52, Sex: 'Male', Company:  { Name: 'Apple', Location: 'USA' } }_ 이고 새 매개변수가 'result'인 경우 사용할 수 있습니다&#x20;

<figure><img src="../../../.gitbook/assets/image (581).png" alt=""><figcaption></figcaption></figure>

### 기타&#x20;

기존 Json 구조를 명령으로 구분 분석하는 것을 지원합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1722).png" alt=""><figcaption></figcaption></figure>
