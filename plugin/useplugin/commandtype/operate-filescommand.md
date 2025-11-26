# 서버 파일 관리 (Operate Filescommand)

서버 파일 관리 플러그인은 서버단 파일의 삭제, 복사 및 파일 정보를 취득할 수 있습니다.&#x20;

이 명령은 서버 단 명령에서만 사용할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1582).png" alt=""><figcaption></figcaption></figure>

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/OperateFilesCommand.zip">OperateFilesCommand.zip</a></td></tr><tr><td>v 9.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/OperateFilesCommand.zip">OperateFilesCommand.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/OperateFilesCommand.zip">OperateFilesCommand.zip</a></td></tr><tr><td>v 7. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7_Plugin_20210722/OperateFilesCommand.zip">OperateFilesCommand.zip</a></td></tr></tbody></table>

### 사용방법&#x20;

서버단 명령실행에서는 파일의 삭제, 복사 및 파일 정보를 취득할 수 있습니다.&#x20;

#### 파일 삭제&#x20;

서버에서 파일 경로를 설정 하고 명령을 실행하면 해당 경로의 파일이 삭제됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (740).png" alt=""><figcaption></figcaption></figure>

#### 파일 복사&#x20;

서버의 특정 파일을 특정 위치에 복사 파일 경로를 설정한 후 이 명령어를 실행하면 파일을 복사하여 다른 경로로 이동시킵니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (643).png" alt=""><figcaption></figcaption></figure>

#### 파일 이동&#x20;

서버의 특정 파일을 특정 위치로 파일 경로를 설정 한후, 이 명령어를 실행하면 파일을 다른 경로로 이동 시킵니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (645).png" alt=""><figcaption></figcaption></figure>

#### 파일 이름 변경&#x20;

서버단 파일 이름을 변경합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>

#### 파일 정보 보기&#x20;

서버에 있는 특정 파일의 이름을 가져옵니다.&#x20;

* 파일 경로  : 파일의 경로&#x20;
* 파일 정보 종류

&#x20;     . 파일 이름: 예: "c:\aaa\bbb\abc.txt" 결과 "abc.txt"

&#x20;     . 파일 확장자: 예: "c:\aaa\bbb\abc.txt" 결과 ".txt"

&#x20;     . 폴더 경로: 예: "c:\aaa\bbb\abc.txt"는 "c:\aaa\bbb"가 됩니다.

&#x20;     . 작성 시

&#x20;     . 마지막 수정 시간

&#x20;     . 파일 존재 여: 파일이 존재하는 경우 결과는 "True"이고 그렇지 않으면 "False"입니다.

&#x20;     . 파일크기: 파일의 파일 크기입니다. 단위는 바이트입니다.

* 결과 저장 파라미터 이름:  명령에서 사용할 수 있도록 결과 정보를 파라미에 저장합니다.

특정 파일이 존재하지 않는 경우. "CreateDateTime", "LastModifyDateTime", "FileSize"를 가져오면 예외가 발생합니다.

<figure><img src="../../../.gitbook/assets/image (1908).png" alt=""><figcaption></figcaption></figure>

#### 파일 다운로드&#x20;

파일 경로와 다운로드 시 파일 이름을 설정하고 이 명령을 실행하면 이 경로의 파일을 다운로드 합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (894).png" alt=""><figcaption></figcaption></figure>

#### 파일에 컨텐츠 저장&#x20;

컨텐츠를 지정된 파일, 콘텐츠: 텍스트 또는 수식(서버 명령 매개변수)에 저장합니다. 세 가지 유형의 콘텐츠가 있습니다.

* 간단한 텍스트: 파일에 쓰기만 하면 됩니다.
* 개체: 데이터베이스에서 쿼리한 데이터와 같이 이동 가능한 유형은 json을 통해 데이터를 직렬화하고 결과를 파일에 씁니다.
* 파일 스트림(스트림): 이것은 Http 요청 명령을 보내는 것으로부터의 결과로 파일 스트림이 될 수 있으며 이동 가능한 유형은 스트림을 파일에 저장합니다.

<figure><img src="../../../.gitbook/assets/image (2187).png" alt=""><figcaption></figcaption></figure>

#### 폴더 생성&#x20;

폴더 경로를 입력하고 명령을 실행하면 폴더를 생성합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (611).png" alt=""><figcaption></figcaption></figure>

#### 폴더 삭제&#x20;

폴더 경로를 입력하고 명령을 실행하면 해 폴더를 삭제합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (626).png" alt=""><figcaption></figcaption></figure>

#### 폴더에 있는 파일 검색&#x20;

폴더 경로를 입력한 후, 결과 저장 파라미터 이름을 설정하고 명령을 수행하면 해당 폴더에 있는 파일을 검색할 수 있습니다. 검색 결과는 결과  저장 파라미터 이름에 저장됩니다.&#x20;

하위 폴더 포함을 체크하면 하위 폴더에서도 파일 검색이 진행됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (2162).png" alt=""><figcaption></figcaption></figure>

#### 데이터베이스에서 파일 정보 검색&#x20;

데이터베이스 첨부파일의 값을 입력하고 명령을 실행하 해당 첨부파일이 데이터베이스에서 검색됩니다.&#x20;

결과 저장 파라미터 이름에 검색 결과가 저장됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (508).png" alt=""><figcaption></figcaption></figure>

#### ZIP 폴더&#x20;

폴더경로와 ZIP파일 경로를 입력하고 명령을 실행하면 입력한 폴더경로가 ZIP파일로 압축되어 ZIP 파일경로에 해당 ZIP파일이 생성됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1430).png" alt=""><figcaption></figcaption></figure>
