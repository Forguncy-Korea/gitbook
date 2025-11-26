# 작업 셀

현재 페이지로 가져온 후 셀 이름을 통해 셀 개체를 가져오면 셀 값 수정, 셀 활성화 또는 비활성화와 같은 셀을 조작할 수 있습니다.

## 셀 조작&#x20;

셀 개체를 가져오면 셀을 조작하고 셀 개체에 대한 여러 메서드를 구현할 수 있습니다.&#x20;

예를 들어 setValue 메서드를 사용하여 지정된 셀(myCell)의 값을 설정합니다.

```javascript
// 현재 페이지 가져오기
var page= Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
  var textCell = page.getCell("myCell");
//지정된 셀의 값 설정
textCell.setValue("이동 가능한 유형");
```

![](https://help.grapecity.com.cn/download/thumbnails/56532211/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1611021619000\&api=v2) 디자이너의 페이지에서 셀 범위를 선택하고 이름을 "myCell"으로 지정합니다.

<figure><img src="../../.gitbook/assets/image (354).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532211/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1611021619000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../.gitbook/assets/image (1086).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532211/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021619000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행한 후 버튼을 클릭하면 지정된 셀의 값이 설정됩니다.

<figure><img src="../../.gitbook/assets/image (2138).png" alt=""><figcaption></figcaption></figure>

## 셀 이벤트

셀을 가져온 후 셀에 대한 이벤트를 바인딩할 수도 있습니다.

예를 들어 bind 메서드를 사용하여 버튼에 클릭 이벤트를 추가하고 버튼을 클릭하면 경고 상자가 나타납니다.

```javascript
//클릭 이벤트 핸들러를 버튼에 바인딩
var onClick = function(arg) {
     alert("이동 가능한 타입");
}
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 button이라는 이름의 버튼을 가져옵니다.
var cell = page.getCell("button");
//셀의 이벤트 바인딩
cell.bind("click", onClick);
```

![](https://help.grapecity.com.cn/download/thumbnails/56532211/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1611021619000\&api=v2) 디자이너의 페이지에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 이름을 "button"으로 지정합니다.

<figure><img src="../../.gitbook/assets/image (1182).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532211/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1611021619000\&api=v2) 페이지 설정에서 \[페이지 로딩 시 명령 편집]을 클릭하고 명령을 JavaScript 명령으로 선택하고 JavaScript 코드를 입력합니다.

<figure><img src="../../.gitbook/assets/image (1747).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532211/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021619000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 클릭하면 경고 상자가 나타납니다.

<figure><img src="../../.gitbook/assets/image (1500).png" alt=""><figcaption></figcaption></figure>

