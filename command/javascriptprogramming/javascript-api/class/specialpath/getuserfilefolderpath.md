# getUserFileFolderPath 메서드

#### 메서드 <a href="#getuserfilefolderpath-fang-fa-fang-fa" id="getuserfilefolderpath-fang-fa-fang-fa"></a>

&#x20;  SpecialPath.getUserFileFolderPath()

#### 설명 <a href="#getuserfilefolderpath-fang-fa-miao-shu" id="getuserfilefolderpath-fang-fa-miao-shu"></a>

사용자 파일의 저장소 경로를 가져옵니다.

#### **매개 변수** <a href="#getuserfilefolderpath-fang-fa-can-shu-shuo-ming" id="getuserfilefolderpath-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### **반환값**  <a href="#getuserfilefolderpath-fang-fa-fan-hui-zhi" id="getuserfilefolderpath-fang-fa-fan-hui-zhi"></a>

string&#x20;

#### 예제 <a href="#getuserfilefolderpath-fang-fa-shi-li" id="getuserfilefolderpath-fang-fa-shi-li"></a>

다음 예제 코드에서는 getUserFileolderPath 메서드를 사용하여 사용자 파일의 저장소 경로를 가져옵니다.

```
// 도움말 메소드 얻기
var helper = Forguncy.Helper;
//사용자 파일의 저장 경로 가져오기
var path = helper.SpecialPath.getUserFileFolderPath();
// 폴더 경로를 보여주는 경고 상자가 나타납니다.
alert(path);
```

#### 사용 예제 <a href="#getuserfilefolderpath-fang-fa-shi-li" id="getuserfilefolderpath-fang-fa-shi-li"></a>

1. 페이지에서 셀 범위를 선택하고, 셀 유형을 버튼으로 설정하고, 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고, JavaScript 코드를 입력합니다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (1865).png" alt=""><figcaption></figcaption></figure>

2. 페이지를 실행합니다.버튼을 클릭하면 사용자 파일의 저장 경로가 표시된 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1660).png" alt=""><figcaption></figcaption></figure>
