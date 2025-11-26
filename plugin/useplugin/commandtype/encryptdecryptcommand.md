# 암호화 및 복호화 알고리즘(EncryptDecryptCommand)

서버가 다른 소프트웨어와 연결되면 반환 값을 암호화해야 하는 경우가 많은데 이 플러그인은 MD5 및 Base64와 같은 다양한 암호화 요구 사항을 완벽하게 해결할 수 있습니다.&#x20;

이 플러그인은 서버단 명령에서만 사용할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1881).png" alt=""><figcaption></figcaption></figure>

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/EncryptDecryptCommand.zip">EncryptDecryptCommand.zip</a></td></tr><tr><td>v 9.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/EncryptDecryptCommand.zip">EncryptDecryptCommand.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/EncryptDecryptCommand.zip">EncryptDecryptCommand.zip</a></td></tr></tbody></table>

### 사용 방법&#x20;

1. 플러그인을 다운로드합니다.
2. Forguncy Builder에서 설치하고 Forguncy Builder를 다시 실행합니다.
3. 서버단 명령에서 아래와 같이 설정합니다.&#x20;

&#x20; 3-1. 서버단 명령 실행 창에서 파라미터를 설정합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1285).png" alt=""><figcaption></figcaption></figure>

&#x20; 3-2. 서버단 명령 실행 창에서 반환값을 설정합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (2073).png" alt=""><figcaption></figcaption></figure>

&#x20; 3-3. 서버단 명령 실행 창에서 명령을 다음과 같이 설정합니다.&#x20;

&#x20;  \- 명령 선택 : MD5 암호화&#x20;

&#x20;  \- Source : SourceCode&#x20;

&#x20;  \- 알고리즘 : 소문자 16  (대문자 16, 소문자 16, 대문자 32, 소문자 32 총 4가지 암호화 방법 제공)

&#x20;  \- 결과를 파라미터로 반환 : Result&#x20;

<figure><img src="../../../.gitbook/assets/image (1352).png" alt=""><figcaption></figcaption></figure>

4\. 실행하면 아래와 같이 암호화 코드를 반환합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1928).png" alt=""><figcaption></figcaption></figure>

## 암호화 유형&#x20;

### MD5 암호화의 16비트와 32비트의 차이점 &#x20;

#### 적용시나리오&#x20;

사용자 비밀번호, 요청 매개변수, 파일 확인 등&#x20;

#### 차이점&#x20;

16비트 암호화는 32비트 MD5 해시에서 중간 16비트를 추출하는 것으로, 32비트 암호화에 비해 16비트 암호화는 해독하기가 더 어렵습니다. 32비트를 크랙할 필요가 없으며 암호화 후 바로 비교할 수 있습니다.



### SHA-1 암호화 명령&#x20;

사용 방법은 기본적으로 MD5와 동일합니다.  사용법은 기본적으로 MD5와 동일하지만 Base64는 암호화 뿐만 아니라 복호화도 지원한다는 차이점이 있습니다.



### HMAC 암호화 명령 사용 지침&#x20;

HMAC 암호화 알고리즘은 암호화된 해시 기능과 공유 키를 기반으로 하는 보안 메시지 인증 프로토콜입니다.

HMAC 암호화 알고리즘은 메시지 무결성을 위한 키 기반 검증 방식이며 보안은 Hash 암호화 알고리즘을 기반으로 하며 전송 중 데이터 가로채기 및 변조를 효과적으로 방지하고 데이터의 무결성, 신뢰성 및 보안을 유지합니다.

양 당사자가 키를 공유하고, 알고리즘에 동의하고, 메시지에 대해 해시 연산을 수행하여 고정 길이 인증 코드를 형성해야 합니다.

통신의 양 당사자는 인증 코드를 확인하여 메시지의 유효성을 결정합니다.

HMAC 암호화 알고리즘은 암호화, 전자 서명, 메시지 확인 등에 사용할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (913).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="229">항목 </th><th>유형 </th><th>설명 </th></tr></thead><tbody><tr><td>Source </td><td>입력 값</td><td>일반 텍스트 문자열 전달</td></tr><tr><td>Secret</td><td>입력 값</td><td>사용자 지정 키 전달</td></tr><tr><td>알고리즘 </td><td>입력 값</td><td>암호화 방법 선택(HMACSHA1, HMACSHA256, HMACSHA512, HMACMD5), </td></tr><tr><td>결과를 파라미터로 반환 </td><td>출력 값</td><td>암호화된 암호문을 새 매개변수에 전달</td></tr></tbody></table>

