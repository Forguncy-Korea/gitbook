# Linux 시스템에서 서버(server) 설치

Linux 시스템에 포건시서버 설치를 지원합니다. 설치 후 애플리케이션을 Linux 서버에 배포할 수 있습니다.

Windows 시스템에서 애플리케이션에 액세스하거나 관리 콘솔에 로그인하여 애플리케이션을 관리할 수 있습니다.



### 지원되는 Linux 시스템 <a href="#zhi-chi-de-linux-xi-tong" id="zhi-chi-de-linux-xi-tong"></a>

* Ubuntu 16.04
* Ubuntu 18.04
* CentOS 7(1804)
* RedHat 7.6
* Kirin v7 v7 update6(20190820)
* 갤럭시 기린 v10 Sp2(20210524)



### Linux에 포건시 서버 설치&#x20;

**1.** Linux 설치 패키지 "ForguncyServerService\_kr\_online.tar"를 다운로드한 후 xFTP와 같은 파일 전송 소프트웨어를 사용하여 설치 패키지를 Linux 시스템 시스템(예: tmp 폴더)에 저장합니다.

**2.** Linux 시스템에 이동식 서버를 설치합니다. Linux 원격 호스트에 접속하려면 SSH를 미리 설치해야 합니다.

다음은 XShell을 사용하여 Linux 원격 호스트에 연결하고 명령줄을 통해 이동식 서버를 설치하는 방법을 예로 들어 설명합니다.

명령줄을 사용하여 tmp 폴더로 이동합니다.

```bash
cd /tmp
```

**3.** 명령줄을 통해 파일의 압축을 풉니다.

```undefined
sudo tar -xvf ForguncyServerService_kr_online.tar
```

**4.**  압축이 풀린 .sh 파일을 명령줄을 통해 실행하여 이동식 서버를 설치합니다.

```undefined
sudo bash installForguncy_cn.sh
```

실행 후 .netCore 소프트웨어 패키지와 GDI+ 소프트웨어 패키지가 설치되고, 이동식 서버가 설치됩니다.

설치 과정은 약 몇 분 정도 소요됩니다.

**5.** 다음과 같은 내용이 출력되면 포건시서버 설치가 완료된 것입니다.

<figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/80953382/image2020-9-22_13-33-17.png" alt=""><figcaption></figcaption></figure>

Windows 시스템에서는 빨간색 상자의 URL에 접속하여 관리 콘솔에 들어갑니다.

<figure><img src="../../.gitbook/assets/image (106).png" alt=""><figcaption></figcaption></figure>
