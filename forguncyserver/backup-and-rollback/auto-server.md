# 서버 측 자동 백업 및 복원

포건시 서버는 자동 백업을 지원하며, 자동 백업을 설정하면 모든 응용프로그램 사용자 정보, 데이터테이블등이 백업됩니다.

## 백업 예약 설정&#x20;

관리 콘솔에서 앱을 선택하여 앱의 일반 설정 페이지로 들어갑니다.

"게시 시 백업 자동 설정"에서 "데이터베이스 게시 시 자동 백업 서버 적용 재정의"를 선택하고 자동 백업 경로를 설정합니다.

자동 백업 경로를 설정한 후 디자이너에서 애플리케이션을 퍼블리싱할 때 데이터베이스를 덮어쓰면 서버가 자동으로 해당 애플리케이션을 백업합니다.

<figure><img src="../../.gitbook/assets/image (2521).png" alt=""><figcaption></figcaption></figure>

### 예약된 백업 및 복원 <a href="#ding-shi-bei-fen-yu-hai-yuan" id="ding-shi-bei-fen-yu-hai-yuan"></a>

관리 콘솔에서 자동 예약 백업을 구성할 수 있으며, 백업 폴더, 시간, 간격, 최대 백업 횟수를 설정할 수 있습니다.

관리 콘솔에서 "설정->백업 및 복원"을 선택합니다. 예약 백업 구성 영역에서 "예약 백업 켜기"를 선택하고 백업 시간, 백업 간격 일수, 최대 백업 횟수를 설정한 후 "설정 저장"을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2523).png" alt=""><figcaption></figcaption></figure>

설정을 저장한 후, 설정된 시간과 간격에 따라 백업이 진행됩니다.

아래 백업 세트 목록에는 자동 백업과 수동 백업을 포함한 모든 백업이 나열되며, 백업 날짜와 시간, 백업 모드(수동 또는 자동), 백업 모듈(내장된 사용자 정보 또는 애플리케이션)이 나열됩니다.

클릭하면 ![](https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/80953411/image2022-4-12_8-35-16.png)백업 정보를 확장하여 백업 파일 정보를 볼 수 있습니다. 지정된 백업을 복원, 다운로드 또는 삭제할 수 있으며, 지정된 백업에서 모듈을 복원 또는 다운로드할 수 있습니다.

백업 폴더를 열면 애플리케이션 이름을 딴 폴더와 백업된 사용자 정보를 포함하여 백업된 파일도 볼 수 있습니다. "usersBackup-auto-**.fubak"라는 파일은 사용자에 대한 백업 파일입니다. , "**"는 백업 날짜입니다.

### 절감 <a href="#hai-yuan" id="hai-yuan"></a>

#### **복원** <a href="#strong-ying-yong-hai-yuan-strong" id="strong-ying-yong-hai-yuan-strong"></a>

관리 콘솔의 모든 애플리케이션 목록에서 복원이 필요한 웹사이트를 클릭하여 해당 애플리케이션의 일반 설정 페이지로 들어갑니다.

백업 및 복원 영역에서 "복원"을 클릭하고 복원할 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2524).png" alt=""><figcaption></figcaption></figure>

#### 사용자 정보 복원 <a href="#yong-hu-xin-xi-hai-yuan" id="yong-hu-xin-xi-hai-yuan"></a>

관리 콘솔에서 "내부->구성->백업 및 복원"을 선택하여 사용자 계정 정보에 대한 백업 및 복원 인터페이스로 들어갑니다.

복원 영역에서 "복원"을 클릭하고 복원하려는 파일을 선택하십시오.

<figure><img src="../../.gitbook/assets/image (2525).png" alt=""><figcaption></figcaption></figure>
