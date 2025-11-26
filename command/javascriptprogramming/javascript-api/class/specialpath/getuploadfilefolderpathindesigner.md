# getUploadFileFolderPathInDesigner 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366366/blue%20block.png?version=1\&modificationDate=1648092746000\&api=v2) 메서드 <a href="#getuploadfilefolderpathindesigner-fang-fa-fang-fa" id="getuploadfilefolderpathindesigner-fang-fa-fang-fa"></a>

&#x20;  SpecialPath.getUploadFileFolderPathInDesigner()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366366/blue%20block.png?version=1\&modificationDate=1648092746000\&api=v2) 설명 <a href="#getuploadfilefolderpathindesigner-fang-fa-miao-shu" id="getuploadfilefolderpathindesigner-fang-fa-miao-shu"></a>

디자이너에 업로드된 파일의 폴더 경로를 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366366/blue%20block.png?version=1\&modificationDate=1648092746000\&api=v2) **매개 변수** <a href="#getuploadfilefolderpathindesigner-fang-fa-can-shu-shuo-ming" id="getuploadfilefolderpathindesigner-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366366/blue%20block.png?version=1\&modificationDate=1648092746000\&api=v2) **반환값**  <a href="#getuploadfilefolderpathindesigner-fang-fa-fan-hui-zhi" id="getuploadfilefolderpathindesigner-fang-fa-fan-hui-zhi"></a>

string

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366366/blue%20block.png?version=1\&modificationDate=1648092746000\&api=v2) 예제 <a href="#getuploadfilefolderpathindesigner-fang-fa-shi-li" id="getuploadfilefolderpathindesigner-fang-fa-shi-li"></a>

다음 예제 코드에서는 getUploadFileFolderPathInDesigner 메서드를 사용하여 디자이너에 업로드된 파일의 폴더 경로를 가져옵니다.

```
// 도움말 메소드 얻기
var helper = Forguncy.Helper;
//업로드된 파일의 폴더 경로 가져오기
var path = helper.SpecialPath.getUploadFileFolderPathInDesigner();
//업로드된 파일이 있는 폴더 경로를 보여주는 경고 상자 팝업
alert(path);
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366344/blue%20block.png?version=1\&modificationDate=1648092746000\&api=v2) 사용 예제 <a href="#getimageeditoruploadimagefolderpath-fang-fa-shi-li" id="getimageeditoruploadimagefolderpath-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72366330/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092746000\&api=v2)페이지에서 셀 범위를 선택하고, 셀 유형을 버튼으로 설정하고, 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고, JavaScript 코드를 입력합니다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (1335).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366366/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092746000\&api=v2)페이지를 실행합니다.버튼을 클릭하면 업로드된 파일이 있는 폴더의 경로를 보여 주는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (2259).png" alt=""><figcaption></figcaption></figure>
