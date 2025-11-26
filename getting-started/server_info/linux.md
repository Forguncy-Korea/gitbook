# Linux 시스템에서 서버제거

### Linux 시스템에서 포건시 서버 제거 <a href="#xie-zai-linux-xi-tong-shang-de-huo-zi-ge-fu-wu-duan" id="xie-zai-linux-xi-tong-shang-de-huo-zi-ge-fu-wu-duan"></a>

포건시  서버를 제거하려면 다음 명령줄을 사용하십시오. 삭제 중에 사용자 데이터는 삭제되지 않습니다.

```undefined
sudo bash installForguncy_kr.sh -r
```

### 일반적으로 사용되는 명령줄 <a href="#chang-yong-ming-ling-xing" id="chang-yong-ming-ling-xing"></a>

서비스 다시 시작

```undefined
sudo service ForguncyServerService restart
```

서비스 중단

```vbnet
sudo service ForguncyServerService stop
```

서비스 시작

```sql
sudo service ForguncyServerService start
```

상태 보기

```lua
sudo service ForguncyServerService status
```

### 글꼴 설치 <a href="#an-zhuang-zi-ti" id="an-zhuang-zi-ti"></a>

애플리케이션을 Linux 시스템에 배포한 후 Linux 시스템에 글꼴이 설치되어 있지 않으면 애플리케이션의 페이지/테이블/피벗 테이블을 Excel/PDF로 내보낼 때 잘못된 문자가 나타납니다. 따라서 Linux 시스템에 필요한 글꼴을 설치해야 합니다.

**단계**

**1.** 폴더를 만듭니다. 예를 들어 폴더 이름은 "cn"입니다.

```bash
sudo mkdir /usr/share/fonts/truetype/cn -p
```

기존 폴더 "/usr/share/fonts/"를 사용할 수도 있습니다.

**2.** 포건시에 글꼴이 저장되어 있는 "/opt/ForguncyServer/Fonts/" 폴더에 필요한 글꼴 파일을 업로드합니다.

글꼴 파일은 Xftp와 같은 파일 전송 소프트웨어를 사용하여 전송할 수 있습니다.

**3.** 생성된 "cn" 폴더에 폰트 파일을 복사하세요.

```bash
sudo cp -r /opt/ForguncyServer/Fonts/* /usr/share/fonts/truetype/cn
```

**4.** "cn" 폴더의 읽기 및 쓰기 권한을 설정합니다.

```bash
sudo chmod 755 /usr/share/fonts/truetype/cn -R
```

**5.** 글꼴 캐시를 새로 고칩니다.

**sudo fc-cache -f -v**

fc-cache를 찾을 수 없으면 Fontconfig를 설치하세요.

Ubuntu:

```undefined
sudo apt install fontconfig
```

CentOS 7, RedHat 7.6, Kirin:

```undefined
sudo yum install fontconfig
```

### <br>
