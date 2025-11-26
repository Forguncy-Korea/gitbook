# deleteUser메서드

### 메서드&#x20;

Forguncy.deleteUser(userName, successCallback, failCallback)

### 설명&#x20;

이 메서드를 사용하여 지정된 사용자를 제거 합니다.

### 매게변수&#x20;



<table><thead><tr><th>매개변수 </th><th width="149.33333333333331">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>userName</td><td>string</td><td>사용자 이름입니다.</td></tr><tr><td>successCallback</td><td>function</td><td>함수를 성공적으로 콜백했습니다.</td></tr><tr><td>errorCallback</td><td>function</td><td>매개 변수에 오류 메시지가 포함된 콜백 함수가 실패했습니다.</td></tr></tbody></table>

###

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서는 deleteUser 메서드를 통해 지정된 사용자가 제거됩니다.

<pre class="language-javascript"><code class="lang-javascript">// 지정된 사용자 삭제
Forguncy.deleteUser(
  //사용자 지정
<strong>  "양지은",
</strong>  //삭제가 성공하면 삭제가 성공했다는 경고창이 뜹니다.
  function () {
   alert("성공적으로 삭제되었습니다.")
<strong>  },
</strong>  //삭제에 실패하면 경고창이 뜨면서 실패 정보를 보여줍니다.
  function (error) {
   alert(error)
  }
);
</code></pre>

### 사용예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364658/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092718000\&api=v2) 페이지에서 범위를 선택하고 셀 유형을 로그인한 사용자로 설정하고 사용자 정보 보기를 테이블에 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72364658/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092718000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (647).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364658/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092718000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 관리자를 사용하여 로그인한 후 페이지에서 삭제 버튼을 클릭하면 삭제가 성공한다는 경고 상자가 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (610).png" alt=""><figcaption></figcaption></figure>
