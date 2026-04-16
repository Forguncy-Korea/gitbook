# PageDefaultDataLoaded 이벤트

#### 이벤트 <a href="#pagedefaultdataloaded-shi-jian-shi-jian" id="pagedefaultdataloaded-shi-jian-shi-jian"></a>

&#x20;  Forguncy.PageEvents.PageDefaultDataLoaded

#### 설명 <a href="#pagedefaultdataloaded-shi-jian-miao-shu" id="pagedefaultdataloaded-shi-jian-miao-shu"></a>

이 이벤트는 페이지가 로드되고 모든 데이터가 로드될 때 트리거됩니다.

#### **반환값**  <a href="#pagedefaultdataloaded-shi-jian-fan-hui-zhi" id="pagedefaultdataloaded-shi-jian-fan-hui-zhi"></a>

String

#### 예제 <a href="#pagedefaultdataloaded-shi-jian-shi-li" id="pagedefaultdataloaded-shi-jian-shi-li"></a>

다음 예제 코드에서는 bnd 메서드를 사용하여 페이지에 PageDefaultDataLoaded 이벤트를 바인딩하고 페이지가 로드되고 모든 데이터가 로드될 때 경고 상자가 나타납니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//바인드 페이지 이벤트
page.bind("pageDefaultDataLoaded", function (arg1, arg2) {
// 페이지의 페이지 이름을 보여주는 팝업이 나타납니다.
alert(arg2.pageName);
});
```

**사용 예제**&#x20;

1. 페이지 설정에서 JavaScript 파일을 업로드하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1749).png" alt=""><figcaption></figcaption></figure>

2. 페이지를 실행하면 페이지가 로드될 때 페이지 1의 페이지 이름을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (664).png" alt=""><figcaption></figcaption></figure>
