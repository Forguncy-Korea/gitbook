# 지정된 페이지의 JavaScript 파일 등록

각 페이지는 이 페이지의 특수 논리를 처리하기 위해 자체 JavaScript 파일을 등록할 수 있습니다.

{% hint style="info" %}
* 파일에 중국어가 포함된 경우 파일이 유니코드 인코딩을 사용하고 있는지 확인합니다.
* 라이브 그리드에는 JQuery 3.2.1 라이브러리가 내장되어 있으며 스크립트에서 직접 JQuery 기능을 사용할 수 있습니다.
{% endhint %}

## **지정된 페이지의 JavaScript 파일을 등록** <a href="#id-zhu-ce-zhi-ding-ye-mian-de-javascript-wen-jian-2.-zhu-ce-zhi-ding-ye-mian-de-javascript-wen-jian" id="id-zhu-ce-zhi-ding-ye-mian-de-javascript-wen-jian-2.-zhu-ce-zhi-ding-ye-mian-de-javascript-wen-jian"></a>

JavaScript 파일을 지정할 페이지를 선택하고 속성 설정 영역에서 \[페이지 설정] 탭을 선택하고 \[JavaScript 파일] 영역을 클릭하여 JavaScript 파일을 업로드합니다.

업로드가 완료되면 JavaScript를 클릭하고 삭제하고 편집할 수 있습니다.

![](<../../../.gitbook/assets/image (354).png>)

1. 디자이너의 페이지에서 셀 범위를 선택하고 셀 유형을 단추로 설정하고 이름을 "button"으로 지정합니다.
2. &#x20;페이지 설정에서 JavaScript 파일 아래의 업로드 아이콘을 클릭하여 JavaScript 파일을 업로드합니다.

<figure><img src="../../../.gitbook/assets/image (1532).png" alt=""><figcaption></figcaption></figure>

```javascript
//클릭 이벤트 핸들러를 버튼에 바인딩
var onClick = function(arg) {
    alert("이동가능한타입");
}
//현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 button이라는 이름의 버튼을 가져옵니다.
var cell = page.getCell("button");
//셀의 이벤트 바인딩
cell.bind("click", onClick);
```

3. &#x20;편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 클릭하면 경고 상자가 나타납니다.

<figure><img src="../../../.gitbook/assets/image (2185).png" alt=""><figcaption></figcaption></figure>
