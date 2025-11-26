# 사용자 정의 JavaScript 지정

셀에 명령을 설정하거나 페이지가 로드될 때 명령을 편집하려면 명령을 \[자바스크립트로 직접 프로그래밍하]]으로 설정한 다음 JavaScript 코드(지정된 요소의 사용자 정의 JavaScript)를 편집할 수 있습니다.

## 사용자 정의 자바 스크립트 지정&#x20;

지정된 요소에 사용자 정의 JavaScript를 설정하는 방법에 대해 설명합니다.

![](https://help.grapecity.com.cn/download/thumbnails/56532167/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1611021619000\&api=v2) 디자이너의 페이지에서 셀 범위를 선택하고 이름을 "myCell"으로 지정합니다.

<figure><img src="../../../.gitbook/assets/image (1501).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532167/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1611021619000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../.gitbook/assets/image (676).png" alt=""><figcaption></figcaption></figure>

샘플 코드에서 setValue 메서드를 사용 하 여 지정 된 셀 (myCell)의 값을 설정 합니다.

```javascript
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
  var textCell = page.getCell("myCell");
//지정된 셀의 값 설정
textCell.setValue("이동 가능한 유형");
```

![](https://help.grapecity.com.cn/download/thumbnails/56532167/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021619000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행한 후 버튼을 클릭하면 지정된 셀의 값이 설정됩니다.

<figure><img src="../../../.gitbook/assets/image (811).png" alt=""><figcaption></figcaption></figure>
