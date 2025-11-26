# 응용 프로그램 수준 JavaScirpt 파일 등록

일부 JavaScript 파일은 여러 페이지 또는 모든 페이지에서 공유되며 포건시 빌더의 설정 페이지에 전체 응용 프로그램 수준 JavaScript 파일을 업로드할 수 있습니다.

로컬 JavaScript 파일을 업로드하거나 URL 주소를 통해 웹에서 직접 JavaScript 파일을 로드할 수 있습니다.

## 응용 프로그램 수준 JavaScirpt파일 등록하기&#x20;

\[파일-> 옵션-> JavaScript/CSS 제작 관]를 선택하고 \[JavaScript 파일 관리] 영역에서 \[링크 추가], \[파일 업로드] 또는 \[빈 파일 생성]을 선택합니다.

<figure><img src="../../../.gitbook/assets/image (751).png" alt=""><figcaption></figcaption></figure>



* 링크 추가: 네트워크에서 JavaScript 파일을 지정합니다. \[저장]을 클릭하면 JavaScript 파일이 URL로 표시됩니다.
* 파일 업로드: 로컬 JavaScript 파일을 추가합니다.
* 빈 파일 생성: 새 JavaScript 파일을 만듭니다.

JavaScript 파일을 업로드한 후 파일 이름을 클릭한 후 JavaScript 파일을 삭제, 위로 이동, 아래로 이동, 이름 바꾸기 및 편집할 수 있습니다.![](https://help.grapecity.com.cn/download/thumbnails/56532102/image2018-2-1_14-24-21.png?version=1\&modificationDate=1611021618000\&api=v2)

다음은 응용 프로그램 수준 JavaScript 파일을 등록하고 사용하는 방법을 보여 줍니다.

![](https://help.grapecity.com.cn/download/thumbnails/56532102/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1611021618000\&api=v2) 두 셀 범위를 선택하고 셀 유형을 텍스트 상자로 설정합니다.

<figure><img src="../../../.gitbook/assets/image (578).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532102/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1611021618000\&api=v2) \[파일-> 옵션-> JavaScript/CSS]를 선택하고 \[JavaScript 파일 관리] 영역에서 \[파일 업로드]를 선택하여 JavaScript 파일을 업로드합니다.

<figure><img src="../../../.gitbook/assets/image (2169).png" alt=""><figcaption></figcaption></figure>

코드는 다음과 같습니다.

```javascript
function Add(num1, num2){
   var total = num1 + num2;
   return total;
}
```

![](https://help.grapecity.com.cn/download/thumbnails/56532102/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021618000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 이름을 "button"으로 지정합니다. 명령을 편집하고, 명령을 JavaScript 명령으로 설정하고, JavaScript 코드를 입력합니다.

<figure><img src="../../../.gitbook/assets/image (1390).png" alt=""><figcaption></figcaption></figure>

```javascript
//현재 페이지 가져오기
var page=Forguncy.Page;
//페이지의 셀을 가져옵니다.；
var cell1=page.getCell("cell1");
var cell2=page.getCell("cell2");
//셀의 값 가져오기 
var c1=cell1.getValue();
var c2=cell2.getValue();
//추가 함수 호출 
var sum=Add(c1,c2);
//경고 상자 팝업
alert(sum);
```

![](https://help.grapecity.com.cn/download/thumbnails/56532102/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1611021618000\&api=v2) 페이지를 실행한 후 텍스트 상자에 값을 입력한 후 버튼을 클릭하면 계산 결과를 표시하는 경고 상자가 나타납니다.

