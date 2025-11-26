# getContainerCells 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366433/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 메서드 <a href="#getcontainercells-fang-fa-fang-fa" id="getcontainercells-fang-fa-fang-fa"></a>

&#x20;  SubPage.getContainerCells()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366433/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 설명 <a href="#getcontainercells-fang-fa-miao-shu" id="getcontainercells-fang-fa-miao-shu"></a>

&#x20;  자식 페이지의 모든 페이지 컨테이너 유형에 대한 셀을 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366433/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) **매개 변수**  <a href="#getcontainercells-fang-fa-can-shu-shuo-ming" id="getcontainercells-fang-fa-can-shu-shuo-ming"></a>

&#x20;  **없음**&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366433/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) **반환값**  <a href="#getcontainercells-fang-fa-fan-hui-zhi" id="getcontainercells-fang-fa-fan-hui-zhi"></a>

&#x20; [ cell](../cellclass/)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366433/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 예제 <a href="#getcontainercells-fang-fa-shi-li" id="getcontainercells-fang-fa-shi-li"></a>

다음 예제 코드에서는 getContainerCells 메서드를 사용 하 여 하위 페이지의 모든 페이지 컨테이너 형식에 대 한 셀을 가져오고 반환 된 셀 인스턴스의 길이를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//페이지 컨테이너 셀 객체 가져오기
var cell = page.getCell("Container");
//페이지 컨테이너의 자식 페이지 가져오기
var subPage = cell.getContentPage();
//하위 페이지의 모든 페이지 컨테이너 셀 가져오기
var containerCell = subPage.getContainerCells();
//페이지 컨테이너 셀 인스턴스의 길이 가져오기
var len = containerCell.length;
// 셀 인스턴스의 길이를 보여주는 경고 상자 팝업
alert(len);
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366433/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 사용 예제 <a href="#getcontainercells-fang-fa-shi-li" id="getcontainercells-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72366418/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092748000\&api=v2)페이지 1과 페이지 2의 두 페이지를 만듭니다. 페이지 1에서 셀 범위를 선택하고 셀 유형을 페이지 내 컨텐츠가 포함된 셀로 설정하고 이름을 "Container"로 지정하고 하위 페이지를 페이지 2로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1179).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366433/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092748000\&api=v2)  페이지 2에서 두 셀 범위를 선택하고 셀 유형을 페이지 컨테이너로 설정하고 하위 페이지를 페이지 3으로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (951).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366418/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092748000\&api=v2)페이지 1에서 셀 범위를 선택하고, 셀 유형을 버튼으로 설정하고, 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고, JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (2031).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366433/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092748000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 클릭하면 가져온 하위 페이지의 모든 페이지 컨테이너 유형에 대한 셀 인스턴스의 길이를 보여 주는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (506).png" alt=""><figcaption></figcaption></figure>
