# DropBox

DropBox용 클라우드 스토리지 공급자를 등록하면 DropBox에 파일과 폴더를 만들고 다운로드할 수 있습니다.



### 다운로드 링크

{% file src="../../../.gitbook/assets/DropboxProvider (2).zip" %}

### DropBox와의 연동 단계&#x20;

1. **클라우드 스토리지 공급자 등록**\
   사용자 계정 관리 화면 또는 서버 관리 포털에 접속하여 다운로드 링크에서 구한 「DropBox용 클라우드 스토리지 프로바이더」를 등록합니다.
2. **DropBox에서 자격 증명 가져오기**\
   App key 및 App secret을 가져옵니다.
3. **클라우드 스토리지 인증 설정**\
   사용자 계정 관리 화면 또는 서버 관리 포털에 연결하여 인증 설정을 수행합니다.



## 1. 클라우드 스토리지 공급자 등록

1.  포건시 서버 관리자에 로그인합니다. <br>

    * 개발 환경에서는 개발 시 사용자 계정 관리에 로그인하여 로그인합니다.
    * 배포 환경에서는 서버 관리 포털 에 따라 로그인합니다.

    배포환경에서 설명을 합니다. 하지만 개발 환경에서도 방법은 동일합니다. <br>
2.  \[설정>클라우드 저장소 설정]을 선택하여 클라우드 저장소 설정 페이지로 들어갑니다.\
    업로드를 클릭하고 클라우드 저장소 공급자를 선택하고 업로드 후 인증 구성을 수행합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2602).png" alt=""><figcaption></figcaption></figure>


3. 업로드가 완료됩니다.

<figure><img src="../../../.gitbook/assets/image (2603).png" alt=""><figcaption></figcaption></figure>

### 2. DropBox로부터 인증 정보를 취득

아래에서는 Forguncy와 DropBox 간의 협력에 필요한 자격 증명을 얻는 방법을 설명합니다.

> 본 페이지에 게재되고 있는 DropBox의 화면은 작성  당시의 것이며, 화면의 구성이나 순서등은 DropBox의 업데이트등에 의해 바뀌고 있는 경우가 있는 것에 주의해 주세요.

1. **DropBox의 앱 콘솔에 로그인합니다.**\
   [https://www.dropbox.com/developers/apps](https://www.dropbox.com/developers/apps)![](https://docs.forguncy.com/v10/Media/external-link.png)
2.  **새 앱 콘솔에 앱을 만듭니다.**\
    (기존 앱을 사용하는 경우이 단계를 건너 뜁니다.)

    \[Create app]를 선택합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2604).png" alt=""><figcaption></figcaption></figure>

    다음과 같이 설정합니다. (Name your app는 임의의 이름을 설정하십시오)<br>

    <figure><img src="../../../.gitbook/assets/image (2605).png" alt=""><figcaption></figcaption></figure>



    **3. App key와 App secret을 만듭니다.**<br>

    \[Settings]에서 \[Redirect URIs]를 다음과 같이 입력하고 \[Add] 버튼을 클릭합니다.

    * 개발 시 사용자 계정 관리의 경우

```
http: //localhost:<포트 번호>/Forguncy/CloudStorageProvider/OAuthCallback
```

&#x20;     포트 번호는 [응용 프로그램 설정](https://docs.forguncy.com/v10/applicationsettings.html) 의 "개발 시 사용자 이름 계정 관리 포트 번호"입니다.

&#x20;    예) http://localhost:17380/Forguncy/CloudStorageProvider/OAuthCallback<br>

* 서버 관리 포털의 경우&#x20;

```
예) https://<서버 관리 포털의 도메인>:22345/CloudStorageProvider/OAuthCallback
```

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Permissions를 클릭하여 다음 위치를 활성화합니다.

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

\[Settings]를 클릭하고 다음 위치에서 "App key"와 "App secret"를 가져옵니다.

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>



### 3. 클라우드 스토리지 인증 설정&#x20;

1.  **설정 > 클라우드 스토리지 설정 > 인증 설정 > 인증 추가를 클릭합니다.**<br>

    <figure><img src="../../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>


2.  **자격 증명을 설정합니다. 다음 항목을 입력한 후 \[로그인 및 저장]을 클릭합니다.**<br>

    <figure><img src="../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

|  이름      | 임의의 이름을 설정하십시오. 여기에서 지정한 이름이 Forguncy Builder에서 설정할 때 선택 목록으로 표시됩니다. |
| -------- | -------------------------------------------------------------------- |
| 공급자 이름   | DropBox를 선택합니다.                                                      |
| 클라이언트 ID | 「2. DropBox로부터 자격 증명 취득」의 마지막 순서로 작성한 App key를 입력합니다.                |
| 클라이언트 비밀 | "2. DropBox에서 자격 증명 가져오기"의 마지막 단계에서 만든 App secret을 입력합니다.            |
