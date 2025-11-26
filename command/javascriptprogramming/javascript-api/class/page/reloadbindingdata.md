# reloadBindingData 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366187/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 메서드 <a href="#reloadbindingdata-fang-fa-fang-fa" id="reloadbindingdata-fang-fa-fang-fa"></a>

&#x20;  Page.reloadBindingData(tableName)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366187/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 설명 <a href="#reloadbindingdata-fang-fa-miao-shu" id="reloadbindingdata-fang-fa-miao-shu"></a>

현재 페이지에서 사용되는 테이블 및 뷰에서 데이터를 다시 로드합니다.

테이블 설정에서 \[데이터 새로 고침]을 설정할 수 있으며, 이 옵션을 선택하지 않으면 reloadBindingData 메서드를 사용하여 데이터베이스에서 데이터를 다시 로드할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366187/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) **매개 변수** <a href="#reloadbindingdata-fang-fa-can-shu-shuo-ming" id="reloadbindingdata-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="168">매개변수 </th><th width="133">형식 </th><th width="164">필수여부 </th><th>설명 </th></tr></thead><tbody><tr><td>tableName</td><td>string</td><td>YES</td><td>데이터를 다시 로드해야 하는 테이블 이름입니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366187/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) **반환값**  <a href="#reloadbindingdata-fang-fa-fan-hui-zhi" id="reloadbindingdata-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366187/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 예제 <a href="#reloadbindingdata-fang-fa-shi-li" id="reloadbindingdata-fang-fa-shi-li"></a>

다음 예제 코드에서는 reloadBindingData 메서드를 통해 데이터베이스에서 데이터를 다시 로드합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//데이터베이스에서 데이터를 다시 로드
page.reloadBindingData("직원 테이블");
```



#### Forguncy 사용 예제

1. 이번 예제에서는 페이지를 생성하기 전에 데이터베이스 테이블을 한 개 생성합니다.\
   내용은 대충 만들어 보고 싶으셨던 대로 넣으시면 됩니다. 최소 1개의 Column은 생성하셔야 합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-reloadbindingdata01.png" alt=""><figcaption></figcaption></figure>

2\. 페이지를 한 개 생성하고 ListView를 생성합니다. ListView에 위에서 생성한 테이블의 Column을 연결합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-reloadbindingdata02.png" alt=""><figcaption></figcaption></figure>

3\. 버튼을 추가합니다. ‘명령 편집’으로 ‘자바스크립트로 직접 프로그래밍하기’하여 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-reloadbindingdata03.png" alt=""><figcaption></figcaption></figure>

4\. 해당 프로젝트를 실행합니다. 화면에는 아래와 같이 ListView에 연결된 Database 테이블의 내용이 표시됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-reloadbindingdata04.png" alt=""><figcaption></figcaption></figure>

5\. Forguncy 에디어로 돌아가서 데이터베이스 테이블에 아무 내용이나 입력합니다.\
데이터베이스 테이블의 내용을 변경하신 후 CTRL+S 혹은 저장하여 프로젝트를 저장합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-reloadbindingdata05.png" alt=""><figcaption></figcaption></figure>

6\. 다시 웹브라우저로 돌아가서 버튼을 클릭하면 아래와 같이 프로젝트의 데이터 테이블에 수정 후 저장한 내용이 웹브라우저에 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-reloadbindingdata06.gif)
