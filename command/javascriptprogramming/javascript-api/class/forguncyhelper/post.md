# post 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365298/blue%20block.png?version=1\&modificationDate=1648092727000\&api=v2) 메서드 <a href="#post-fang-fa-fang-fa" id="post-fang-fa-fang-fa"></a>

&#x20;  Helper.post(url, param, callback, async)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365298/blue%20block.png?version=1\&modificationDate=1648092727000\&api=v2) 설명 <a href="#post-fang-fa-miao-shu" id="post-fang-fa-miao-shu"></a>

서버에 데이터를 제출합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365298/blue%20block.png?version=1\&modificationDate=1648092727000\&api=v2) **매개 변수**  <a href="#post-fang-fa-can-shu-shuo-ming" id="post-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="139">매개변수 </th><th width="135">형식 </th><th width="105">필수여부</th><th>설명 </th></tr></thead><tbody><tr><td>url</td><td>string</td><td>Yes</td><td>요청이 전송된 URL을 포함하는 문자열입니다.</td></tr><tr><td>param</td><td>any</td><td>Yes</td><td>요청된 데이터를 보냅니다.</td></tr><tr><td>callback</td><td>function</td><td>Yes</td><td>함수를 성공적으로 콜백했습니다.</td></tr><tr><td>async</td><td>boolean</td><td><p></p><p>No</p></td><td>요청이 비동기인지 여부입니다. 기본값은 true입니다.</td></tr></tbody></table>

<br>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365298/blue%20block.png?version=1\&modificationDate=1648092727000\&api=v2) **반환값**  <a href="#post-fang-fa-fan-hui-zhi" id="post-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365298/blue%20block.png?version=1\&modificationDate=1648092727000\&api=v2) 예제입니다 <a href="#post-fang-fa-shi-li" id="post-fang-fa-shi-li"></a>

다음 C# 코드에서 사용자 지정 웹 API 클래스 "MyAPI" 에는 post 특성이 post 특성을 참조하는 post 메서드 "TestPostAPI"가 포함되어 있습니다.

```
public class MyAPI : ForguncyApi
    {
        [Post]
        public void TestPostAPI()
        {
            //포스트 요청 데이터 가져오기
            var form = this.Context.Request.ReadFormAsync().Result;
            var name = form["name"];
            var department = form["department"];
            // 데이터 유형을 문자열로 변환
            string result = Convert.ToString(name) + Convert.ToString(department);
            this.Context.Response.Write(result.ToString());
            //AddTableData 메서드를 사용하여 직원 테이블에 데이터를 추가합니다.
            this.DataAccess.AddTableData("직원테이", new Dictionary<string, object> { { "이름", name }, { "부서", department } });
        }
    }
```

프런트 엔드에서 다음 JavaScript 코드를 사용하여 TestPostAPI 메서드를 호출합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지의 셀 가져오기
var cell1 = page.getCell("name");
var cell2 = page.getCell("department");
// 셀의 값 가져오기
var data = {
    name: cell1.getValue(),
    department: cell2.getValue()
};
// 서버에 요청 보내기
Forguncy.Helper.post("customapi/myapi/testpostapi", data, function () {
    alert("이동 가능한 타입");
});
```
