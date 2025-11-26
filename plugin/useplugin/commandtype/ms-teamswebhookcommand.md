# MS 팀즈에 메세지 전송 (TeamsWebHookCommand)

이 플러그인을 사용하면 MS 팀즈에 메시지 전송을 할 수 있습니다.&#x20;

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/TeamsWebHookCommand.zip">TeamsWebHookCommand.zip</a></td></tr><tr><td>v 9.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/TeamsWebHookCommand.zip">TeamsWebHookCommand.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/TeamsWebHookCommand.zip">TeamsWebHookCommand.zip</a></td></tr><tr><td>v 7. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7_Plugin_20210722/TeamsWebHookCommand.zip">TeamsWebHookCommand.zip</a></td></tr><tr><td>v 6. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6.1_Plugin_20201111/TeamsWebHookCommand.zip">TeamsWebHookCommand.zip</a></td></tr></tbody></table>

### 사용 방법&#x20;

1. 플러그인을 다운로드합니다.
2. Forguncy Builder에서 설치하고 Forguncy Builder를 다시 실행합니다.
3.  팀에서 마우스 오른쪽 메뉴에서 "채널관리"를 클릭합니다. <br>

    <figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>


4.  커넥터에서 \[편집]을 클릭합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

&#x20;4\. Incoming webhook 구성을 클릭합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1372).png" alt=""><figcaption></figcaption></figure>

5\. IncomingWebhook 연결한 이름을 입력한 후, 만들기를 클릭하면 URL이 나옵니다. 해당 URL을 복사합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (546).png" alt=""><figcaption></figcaption></figure>

6\. 서버단 명령 실행에서 아래와 같이 명령을 설정합니다.&#x20;

(버튼 명령, 페이지 명령에서도 사용 가능함 )

* 명령 선택 : Teams 메시지 전송&#x20;
* WebHook URL : 5번에서 복사한 URL
* 내용 : 메시지 내용&#x20;

<figure><img src="../../../.gitbook/assets/image (2075).png" alt=""><figcaption></figcaption></figure>

7\. 해당 명령을 실행하면 아래와 같이 팀즈에 메시지가 보내지는 것을 확인할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (2262).png" alt=""><figcaption></figcaption></figure>
