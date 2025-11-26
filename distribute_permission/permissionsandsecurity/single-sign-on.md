# Single Sign-On

Forguncy에서 작성한 애플리케이션에서 다른 웹 애플리케이션 및 클라우드 서비스 자격 증명을 사용하는 소위 싱글 사인온을 구현하는 경우 인증 공급자의 사용을 고려하십시오.

인증 프로바이더로 실현이 불가능한 경우, 프로그래밍에 의한 커스터마이즈에 의해 싱글 사인온이 가능합니다. 이 섹션에서는 이러한 경우에 싱글 사인온 방법을 설명합니다. 이 기능은 Windows 인증에서는 사용할 수 없습니다.

Forguncy의 인증 연계 기능은 아래 그림과 같은 흐름으로 이루어집니다.

<figure><img src="../../.gitbook/assets/image (2363).png" alt=""><figcaption></figcaption></figure>

## **GetUserToken API 설명**&#x20;

* 요청방법 : POST
* 매개변수 :&#x20;

| 매개변수     | 설명                  |
| -------- | ------------------- |
| userName | 로그인하기 위한 userName   |
| password | Single Sign-On 비밀번호 |

* 반환값

토큰을 성공적으로 얻은 경우 반환된 문자열은 " Error: "로 시작하지 않습니다. 토큰을 얻는 데 실패하면 반환되는 문자열은 오류 메시지이며 "Error: "로 시작합니다. 이는 디버깅과 위치 지정에 편리합니다.



> 사용자이름은 Forguncy의 사용자 관리 시스템에 존재하여야 합니다.&#x20;

## **Single Sign On 설정**



**\[파일] → \[옵션] → \[기타 응용 프로그램과 통합]을 선택하여 \[다른 응용 프로그램의 서명 허용]을 선택합니다.**

다른 응용 프로그램에서 로그인 허용을 선택하지 않으면 사용자의 토큰을 요청할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>

| 설정                 | 설명                                                                                                                                                   |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| 기타 응용 프로그램의 서명 허용  | Single Sign-On을 활성화할지 여부. 기본값은 False입니다.                                                                                                             |
| 로그인 암호             | 사용자 토큰을 얻는 데 필요한 비밀번호입니다. 디자이너를 열면 비밀번호가 무작위로 생성됩니다. Single Sign-On을 허용한 후 파일을 저장하지 않으면 다음에 파일을 열 때 비밀번호가 다시 생성됩니다. 파일을 저장하면 다시 열 때 비밀번호가 변경되지 않습니다. |
| 토큰 시간 제한           | 토큰의 유효 기간.                                                                                                                                           |



Single Sign-On을 설정한 후, 타사(모바일 유형이 아닌) 애플리케이션에 다음 코드를 작성합니다.





```csharp
var baseUrl = "http://localhost:25979/Forguncy";
var userName = "administrator"; 
var password = "7FBqkHeV!4Rw";  // 이 비밀번호는 Single Sign-On 비밀번호입니다.
HttpWebRequest rq = HttpWebRequest.Create(baseUrl + "/SSO/GetUserToken") as HttpWebRequest;
rq.Method = WebRequestMethods.Http.Post;
rq.Accept = "application/json";
rq.ContentType = "application/json";
var loginStr = "{userName:\"" + userName + "\", password:\"" + password + "\"}";
var data = Encoding.UTF8.GetBytes(loginStr);
using (Stream stream = rq.GetRequestStream())
{
    stream.Write(data, 0, data.Length);
}
var response = rq.GetResponse();
var token = new StreamReader(response.GetResponseStream()).ReadToEnd();
if(token.StartsWith("Error:"))
{
    MessageBox.Show(token);
    return;
}
Process.Start(baseUrl + "?token=" + token);
```

>
>
> * 이 기능은 Form 사용자에게만 제공되며 Windows 도메인 사용자는 사용할 수 없습니다.
> * 로그인에 필요한 사용자 이름은 Forguncy 애플리케이션에 이미 존재해야 합니다.
> * 보안을 강화하려면 Single Sign-On 비밀번호가 JavaScript 코드에 나타나서는 안 됩니다. 그래야 유출을 방지할 수 있습니다.



## **배포 후 비밀번호를 직접 수정하세요** <a href="#strong-zhi-jie-xiu-gai-fa-bu-hou-de-mi-ma-strong" id="strong-zhi-jie-xiu-gai-fa-bu-hou-de-mi-ma-strong"></a>

서버의 "C:\Users\Public\Documents\ForguncyServer\ _Application Name_ " 디렉토리에서 "Config.xml" 구성 파일을 찾아 열고 아래 그림과 같이 Password 값을 편집합니다.

<figure><img src="../../.gitbook/assets/image (2601).png" alt=""><figcaption></figcaption></figure>

>
>
> * 비밀번호 노드에 값이 없으면 빌더가 열릴 때 비밀번호가 무작위로 생성된다는 의미입니다.
> * 수정 후에는 웹사이트를 다시 시작해야 합니다.
