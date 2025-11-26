# getMergedColumnInfos 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365511/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) 메서드 <a href="#getmergedcolumninfos-fang-fa-fang-fa" id="getmergedcolumninfos-fang-fa-fang-fa"></a>

&#x20;  ListView.getMergedColumnInfos()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365511/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) 설명 <a href="#getmergedcolumninfos-fang-fa-miao-shu" id="getmergedcolumninfos-fang-fa-miao-shu"></a>

리스트의 모든 열에 대한 정보를 가져옵니다. 행 헤더 열, 선택 열, 숨겨진 열 등을 포함합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365511/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) **매개 변수** <a href="#getmergedcolumninfos-fang-fa-can-shu-shuo-ming" id="getmergedcolumninfos-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365511/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) **반환값**  <a href="#getmergedcolumninfos-fang-fa-fan-hui-zhi" id="getmergedcolumninfos-fang-fa-fan-hui-zhi"></a>

&#x20;  IMergedColumnInfo\[]

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365511/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) 예제 <a href="#getmergedcolumninfos-fang-fa-shi-li" id="getmergedcolumninfos-fang-fa-shi-li"></a>

다음 예제 코드에서는 getMergedColumnInfos 메서드를 사용하여 리스트의 모든 열에 대한 정보를 가져옵니다. 행 헤더 열, 선택 열, 숨겨진 열 등을 포함합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListViews()[0];
//리스트의 모든 컬럼 정보를 얻는다.
var infos=listview.getMergedColumnInfos();
//리스트의 모든 컬럼 정보를 표시하는 경고창 팝업
alert(JSON.stringify(infos, null, " "));
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365511/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) 사용 예제 <a href="#getmergedcolumninfos-fang-fa-shi-li" id="getmergedcolumninfos-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365511/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092730000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365511/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092730000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (444).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365511/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092730000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 테이블 열 정보 버튼을 클릭하면 행 헤더 열, 열 선택, 열 숨기기 등을 비롯한 테이블의 모든 열에 대한 정보가 포함된 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (383).png" alt=""><figcaption></figcaption></figure>
