# setCurrentRow 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366222/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 메서드 <a href="#setcurrentrow-fang-fa-fang-fa" id="setcurrentrow-fang-fa-fang-fa"></a>

&#x20;  Page.setCurrentRow(currentRowParam)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366222/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 설명 <a href="#setcurrentrow-fang-fa-miao-shu" id="setcurrentrow-fang-fa-miao-shu"></a>

테이블 1의 현재 행을 테이블의 첫 번째 행으로 설정하는 등의 현재 행을 설정하면 페이지의 모든 테이블 1의 바인딩 필드에 첫 번째 행에 대한 데이터가 표시됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366222/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) **매개 변수 설명입니다** <a href="#setcurrentrow-fang-fa-can-shu-shuo-ming" id="setcurrentrow-fang-fa-can-shu-shuo-ming"></a>

| 매개변수            | 형식                                                                                                 | 설명          |
| --------------- | -------------------------------------------------------------------------------------------------- | ----------- |
| currentRowParam | [CurrentRowInfoParam](../../forguncyinterface/currentrowinfoparam.md) 또는 CurrentRowInfoPluginParam | 현재 행 정보입니다. |

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366222/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) **반환값**  <a href="#setcurrentrow-fang-fa-fan-hui-zhi" id="setcurrentrow-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366222/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 예제 <a href="#setcurrentrow-fang-fa-shi-li" id="setcurrentrow-fang-fa-shi-li"></a>

&#x20;  **예 1:**

SetCurrentRow 메서드를 사용하여 매개 변수는 [CurrentRowInfoParam](../../forguncyinterface/currentrowinfoparam.md)입니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 행 설정
page.setCurrentRow(
{
//현재 행이 위치한 테이블의 이름
TableName: "직원 테이블",
//현재 행의 쿼리 조건
PrimaryKey: {
ID: 2
}
});
```

**예 2:**

매개 변수는 CurrentRowInfoPluginParam이며 일반적으로 플러그인 개발에 사용됩니다. 예를 들어 다음 코드는 플러그인 명령 SetCurrentRowCommand의 일부입니다.

```
SetCurrentRowCommand.prototype.execute = function () {
Forguncy.Page.setCurrentRow({
QueryCondition: this.CommandParam.CurrentRowInfo,
FormulaCalcContext: this.getFormulaCalcContext()
});
```



#### Forguncy 사용 예제

1. 데이터베이스 테이블을 한 개 생성하고, 테이블 내에 레코드 값을 최소 3개 이상 작성합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-setcurrentrow01.png" alt=""><figcaption></figcaption></figure>

2\. 페이지를 한 개 생성하고, 아래와 같이 데이터 테이블의 Column을 매핑시켜 줍니다.\
※참고 : 데이터 테이블의 컬럼을 화면에 매핑시키는 방법은 아래 그림처럼 끌어다놓기(Drag & Drop) 하시면 됩니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-setcurrentrow02.png" alt=""><figcaption><p><br></p></figcaption></figure>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-setcurrentrow03.gif" alt=""><figcaption></figcaption></figure>

3\. 버튼을 한 개 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령을 이용하여 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-setcurrentrow04.png" alt=""><figcaption></figcaption></figure>

4\. 해당 프로젝트를 실행하면 빈 화면이 나타납니다. 버튼을 입력하면 코드에 입력된 대로 Primary Key인 ID가 2인 정보가 화면에 나타납니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-setcurrentrow05.gif)
