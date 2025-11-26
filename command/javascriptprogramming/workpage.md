# 작업 페이지

페이지 개체는 셀 개체 및 테이블 개체를 가져올 수 있는 포건시의 루트 개체입니다. 페이지의 셀과 테이블은 현재 페이지로 가져온 경우에만 조작할 수 있습니다.

다음 코드를 사용하여 현재 페이지로 가져옵니다.

```javascript
var page = Forguncy.Page;
```

## 작업 페이지&#x20;

#### 페이지 개체를 통해 셀 개체를 가져오기  <a href="#id-cao-zuo-ye-mian-tong-guo-ye-mian-dui-xiang-huo-qu-dan-yuan-ge-dui-xiang" id="id-cao-zuo-ye-mian-tong-guo-ye-mian-dui-xiang-huo-qu-dan-yuan-ge-dui-xiang"></a>

```javascript
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 button이라는 이름의 버튼을 가져옵니다.
var cell = page.getCell("버튼");
```

#### 페이지 개체를 통해 리스트뷰 개체를 가져옵니다 <a href="#id-cao-zuo-ye-mian-tong-guo-ye-mian-dui-xiang-huo-qu-biao-ge-dui-xiang" id="id-cao-zuo-ye-mian-tong-guo-ye-mian-dui-xiang-huo-qu-biao-ge-dui-xiang"></a>

리스트뷰 개체를 가져오면 리스트뷰 개체를 구현하는 여러 가지 방법이 있습니다.

```javascript
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("listview 1");
```

## 페이지 이벤트&#x20;

페이지를 가져온 후에는 Loaded 이벤트, PageDefaultDataLoaded 이벤트 및 PopupClosed 이벤트의 세 가지 이벤트를 지원하는 페이지에 이벤트를 바인딩할 수도 있습니다.

예를 들어 bnd 메서드를 사용하면 페이지에 Loaded 이벤트가 추가되고 페이지가 로드될 때 경고 상자가 나타납니다.

```javascript
// 현재 페이지 가져오기
var page = Forguncy.Page;
//페이지 Loaded 이벤트 바인딩
page.bind("loaded", function(arg1, arg2) {
//1 페이지의 페이지 이름을 보여주는 경고 상자가 나타납니다.
alert(arg2.pageName);
});
```
