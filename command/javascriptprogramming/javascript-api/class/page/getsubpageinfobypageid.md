# getSubPageInfoByPageID 메서드

#### 메서드 <a href="#getsubpageinfobypageid-fang-fa-fang-fa" id="getsubpageinfobypageid-fang-fa-fang-fa"></a>

&#x20;  Page.getSubPageInfoByPageID(pageID)

#### 설명 <a href="#getsubpageinfobypageid-fang-fa-miao-shu" id="getsubpageinfobypageid-fang-fa-miao-shu"></a>

&#x20;  페이지 ID를 통해 하위 페이지를 가져옵니다. 브라우저에서 각 부모 및 자식 페이지에는 고유한 ID가 있습니다. 이 방법은 플러그인에서 사용하기에 더 적합합니다. 사용자는 CellTypeBase.getFormulaCalcContext 및 CommandBase.getFormulaCalcContext 메서드를 통해 페이지 ID를 가져올 수 있습니다.

#### **매개 변수**  <a href="#getsubpageinfobypageid-fang-fa-can-shu-shuo-ming" id="getsubpageinfobypageid-fang-fa-can-shu-shuo-ming"></a>

| 매개변수   |        |             |
| ------ | ------ | ----------- |
| pageID | string | 페이지의 ID입니다. |

#### **반환값**  <a href="#getsubpageinfobypageid-fang-fa-fan-hui-zhi" id="getsubpageinfobypageid-fang-fa-fan-hui-zhi"></a>

&#x20;  SubPage

#### 예제 <a href="#getsubpageinfobypageid-fang-fa-shi-li" id="getsubpageinfobypageid-fang-fa-shi-li"></a>

다음 예제 코드에서는 getSubPageInfoByPageID 메서드를 통해 하위 페이지를 가져옵니다.

```

var pageID = this.getFormulaCalcContext().PageID;
var pageInfo = Forguncy.Page.getSubPageInfoByPageID(pageID);
return pageInfo ? pageInfo.getListView(listViewName) : Forguncy.Page.getListView(listViewName, false);
```
