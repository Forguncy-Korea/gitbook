# getCell 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366401/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 메서드 <a href="#getcell-fang-fa-fang-fa" id="getcell-fang-fa-fang-fa"></a>

&#x20;  SubPage.getCell(name)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366401/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 설명 <a href="#getcell-fang-fa-miao-shu" id="getcell-fang-fa-miao-shu"></a>

셀 이름으로 셀 인스턴스를 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366401/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) **매개 변수** <a href="#getcell-fang-fa-can-shu-shuo-ming" id="getcell-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="201.33333333333331">매개변수 </th><th width="164">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>name</td><td>string</td><td>셀 이름입니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366401/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) **반환값**  <a href="#getcell-fang-fa-fan-hui-zhi" id="getcell-fang-fa-fan-hui-zhi"></a>

&#x20;  [Cell](../cellclass/)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366401/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 예제 <a href="#getcell-fang-fa-shi-li" id="getcell-fang-fa-shi-li"></a>

다음 예제 코드에서는 getCell 메서드를 통해 셀 인스턴스를 가져오고 셀 값을 설정합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지 컨테이너 가져오기
var containerCell = page.getCell("container");
//페이지 컨테이너의 자식 페이지 가져오기
var subPage = containerCell.getContentPage();
//셀 객체 가져오기
var cell = subPage.getCell("myCell");
//셀 값 설정
cell.setValue("이동 가능한 유형");
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366401/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 사용 예제 <a href="#getcell-fang-fa-shi-li" id="getcell-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72366418/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092748000\&api=v2)페이지 1과 페이지 2의 두 페이지를 만듭니다. 페이지 1에서 셀 범위를 선택하고 셀 유형을 페이지 내 컨텐츠가 포함된 셀 설정하고 이름을 "Container"로 지정하고 하위 페이지를 페이지 2로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1179).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366418/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092748000\&api=v2)페이지 2에서 셀 범위를 선택하여 myCell이라는 이름을 지정합니다.

<figure><img src="../../../../../.gitbook/assets/image (425).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366418/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092748000\&api=v2)페이지 1에서 셀 범위를 선택하고, 셀 유형을 버튼으로 설정하고, 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고, JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1630).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366401/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092748000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 클릭하면 가져온 셀에 대한 값이 설정됩니다.

<figure><img src="../../../../../.gitbook/assets/image (1486).png" alt=""><figcaption></figcaption></figure>
