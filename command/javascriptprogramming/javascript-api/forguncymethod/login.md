# logIn 메서드

### 메서드&#x20;

Forguncy.logIn(username, password, rememberMe, successCallback, errorCallback)

### 설명&#x20;

이 메서드를 사용 하 여 지정 된 사용자 이름 및 암호와 연결 된 계정에 로그인 합니다.

### 매개변수&#x20;

<table><thead><tr><th width="178">매개변수 </th><th width="143">형식 </th><th width="70">필수여부 </th><th>설명 </th></tr></thead><tbody><tr><td>username</td><td>string</td><td>Yes</td><td>사용자 이름입니다.</td></tr><tr><td>password</td><td>string</td><td>Yes</td><td>암호입니다.</td></tr><tr><td>rememberMe</td><td>boolean</td><td>No</td><td>브라우저가 현재 사용자를 기억할 수 있도록 할지 여부입니다. 기본값은 false입니다.</td></tr><tr><td>successCallback</td><td>Function</td><td>No</td><td>함수가 성공적으로 콜백되고 값이 비어 있으면 기본적으로 브라우저가 즉시 새로 고쳐집니다.</td></tr><tr><td>errorCallback</td><td>Function</td><td>No</td><td>실패한 콜백 함수입니다.</td></tr></tbody></table>

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서는 logIn 메서드를 사용 하 여 지정 된 사용자 이름 및 암호와 연결 된 계정에 로그인 합니다.

```javascript
Forguncy.logIn("Administrator","123456");
```

### 사용 방법&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364737/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092719000\&api=v2) 페이지에서 셀 범위를 선택하고 셀 유형을 버튼으 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (652).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364737/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092719000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 로그인 버튼 클릭하면 Administrator 사용자로 로그인하고 페이지를 새로 고치면 로그인한 사용자 이름이 페이지에 표시됩니다.
