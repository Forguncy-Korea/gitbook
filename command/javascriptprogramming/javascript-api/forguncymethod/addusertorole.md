# addUserToRole 메서드

### 메서드&#x20;

Forguncy.addUserToRole(userName, roleName, successCallback, failCallback)

### 설명&#x20;

이 메서드를 사용하여 지정 된 그룹에 지정 된 사용자를 추가하여 사용자에 대한 역할을 지정합니다.

### 매개 변수&#x20;

| 매개변수            | 형식       |                                   |
| --------------- | -------- | --------------------------------- |
| userName        | string   | 사용자 이름입니다.                        |
| roleName        | string   | 그룹 이름, 즉 역할 이름입니다.                |
| successCallback | function | 함수를 성공적으로 콜백했습니다.                 |
| failCallback    | function | 매개 변수에 오류 메시지가 포함된 콜백 함수가 실패했습니다. |

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서는 addUserToRole 메서드를 통해 지정된 사용자를 지정된 그룹에 추가합니다.

```javascript
//지정된 그룹에 지정된 사용자 추가
Forguncy.addUserToRole(
  //사용자 지정
  "장산",
  //그룹 지정
  "Administrator",
  //추가에 성공하면 추가 성공을 알리는 경고 상자가 팝업됩니다.
  function () {
    alert("성공적으로 추가되었습니다.")
  },
  //추가 실패시 경고창이 뜨면서 실패 정보를 보여줍니다.
  function (error) {
    alert(error)
  }
);
```

![](https://help.grapecity.com.cn/download/thumbnails/72364590/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092717000\&api=v2) 페이지에서 범위를 선택하고 셀 유형을 로그인한 사용자로 설정하고 사용자 정보 보기를 테이블에 바인딩합니다.

<figure><img src="../../../../.gitbook/assets/image (2076).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364590/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092717000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (1031).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364590/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092717000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 관리자를 사용하여 로그인한 후 페이지에서 그룹에 추가 버튼 클릭하면 성공적으로 추가했다는 알림창이 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (1158).png" alt=""><figcaption></figcaption></figure>
