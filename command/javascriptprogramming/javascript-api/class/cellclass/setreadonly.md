# setReadOnly 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365221/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) 메서드 <a href="#setreadonly-fang-fa-fang-fa" id="setreadonly-fang-fa-fang-fa"></a>

&#x20;  Cell.setReadOnly()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365221/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) 설명 <a href="#setreadonly-fang-fa-miao-shu" id="setreadonly-fang-fa-miao-shu"></a>

셀의 읽기 전용 상태를 설정합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365221/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) **매개 변수** <a href="#setreadonly-fang-fa-can-shu-shuo-ming" id="setreadonly-fang-fa-can-shu-shuo-ming"></a>

| 매개변수       | 형식      | 설명         |
| ---------- | ------- | ---------- |
| isReadOnly | boolean | 읽기 전용인지 여부 |

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365221/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) **반환값**  <a href="#setreadonly-fang-fa-fan-hui-zhi" id="setreadonly-fang-fa-fan-hui-zhi"></a>

any

다음 예제 코드에서는 setReadOnly 메서드를 사용하여 셀(myCell)을 읽기 전용으로 설정합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
var cell = page.getCell("myCell");
//셀을 읽기 전용 상태로 설정
cell.setReadOnly(true);
```

#### 사용 예제   <a href="#setreadonly-fang-fa-fan-hui-zhi" id="setreadonly-fang-fa-fan-hui-zhi"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365221/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092726000\&api=v2) 디자이너의 페이지에서 텍스트 상자로 설정된 셀을 선택하고 이름을 "myCell"로 지정합니다.

#### ![](<../../../../../.gitbook/assets/image (2269).png>) <a href="#setreadonly-fang-fa-shi-li" id="setreadonly-fang-fa-shi-li"></a>



![](https://help.grapecity.com.cn/download/thumbnails/72365221/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092726000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (903).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365221/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092726000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 btn 버튼 클릭하면 텍스트 상자가 읽기 전용으로 설정되고 텍스트 상자에 값을 입력할 수 없습니다.
