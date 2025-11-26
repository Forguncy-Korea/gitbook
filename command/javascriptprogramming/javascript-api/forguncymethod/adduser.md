# addUser 메서드

### 메서드&#x20;

일반 인증 모드에서는 다음 방법을 사용하여 사용자를 추가합니다.

&#x20;  Forguncy.addUser(userName, password, displayName, email, successCallback, failCallback)

도메인 인증 모드에서는 다음 방법을 사용하여 사용자를 추가합니다.

&#x20;  Forguncy.addUser(userName, successCallback, failCallback)

### 설명&#x20;

이 방법을 사용하여 일반 인증 모드를 포함하여 사용자를 추가하고 도메인 인증 모드에서 사용자를 추가합니다.

### 매개변수&#x20;

일반 인증 모드에서 사용자를 추가하는 매개 변수는 다음과 같습니다.



| 매개변수            | 형식       | 설명                                |
| --------------- | -------- | --------------------------------- |
| displayName     | string   | 전체 이름입니다.                         |
| email           | string   | 이메일 주소입니다.                        |
| failCallback    | function | 매개 변수에 오류 메시지가 포함된 콜백 함수가 실패했습니다. |
| password        | string   | 암호입니다.                            |
| successCallback | function | 함수를 성공적으로 콜백했습니다.                 |
| userName        | string   | 사용자 이름입니다.                        |

도메인 인증 모드에서 사용자를 추가하는 매개 변수는 다음과 같습니다.

| 매개 변수           | 형식       | 설명                                |
| --------------- | -------- | --------------------------------- |
| userName        | string   | 사용자 이름입니다.                        |
| successCallback | function | 함수를 성공적으로 콜백했습니다.                 |
| failCallback    | function | 매개 변수에 오류 메시지가 포함된 콜백 함수가 실패했습니다. |

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서 addUser 메서드를 통해 사용자를 추가 합니다.

* 일반 인증 모드에서 사용자 추가:

<pre class="language-javascript"><code class="lang-javascript">//사용자 추가
Forguncy.addUser(
  //사용자 이름
<strong>  "리틀 리",
</strong>  //사용자의 비밀번호
  "123456",
  //사용자의 전체 이름
  "리시",
  //사용자의 이메일
  "lisi@grapecity.com",
  //추가에 성공하면 추가 성공을 알리는 경고 상자가 팝업됩니다.
  function () {
    alert("성공적으로 추가되었습니다.")
  },
  //추가 실패시 경고창이 뜨면서 실패 정보를 보여줍니다.
  function (error) {
    alert(error)
  }
);
</code></pre>

* 도메인 인증 모드에서 사용자 추가:

<pre class="language-javascript"><code class="lang-javascript">//사용자 추가
Forguncy.addUser(
  //사용자 이름
  "리틀 리",
  //추가에 성공하면 추가 성공을 알리는 경고 상자가 팝업됩니다.
  function () {
<strong>    alert("성공적으로 추가되었습니다.")
</strong>  },
  //추가 실패시 경고창이 뜨면서 실패 정보를 보여줍니다.
  function (error) {
    alert(error)
  }
);
</code></pre>

다음은 일반 인증 모드에서 사용자를 추가하는 방법을 보여 드리겠습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72364609/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092717000\&api=v2) 페이지에서 범위를 선택하고 셀 유형을 로그인한 사용자로 설정하고 사용자 정보 보기를 테이블에 바인딩합니다.

<figure><img src="../../../../.gitbook/assets/image (1783).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364609/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092717000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (1484).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364609/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092717000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 관리자를 사용하여 로그인한 후 페이지에서 사용자 추가 버튼 클릭하면 추가가 성공한다는 경고 상자가 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (2108).png" alt=""><figcaption></figcaption></figure>
