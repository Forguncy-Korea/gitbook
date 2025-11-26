# 서버단 알림 생성 및 적용

서버가 클라이언트(브라우저)와 상호 작용하려면 상호 작용 정보를 전달할 수 있는 채널, 즉 "서버 알림"이 필요합니다.<br>

서버단 알림을 사용하여 자동 팝업 할 일 메시지, 인스턴트 메시징, 브라우저 사이트 메시지 및 온라인 고객 서비스와 같은 고급 기능을 실현할 수 있습니다.

서버 알림 기능은 기본적으로 개체 관리자에 표시되지 않는 고급 기능입니다 .서버 알림 앞의 확인란을 선택 하고 "확인"을 클릭하면 개체 관리자에 서버 알림이 표시됩니다.

<figure><img src="../../../../.gitbook/assets/image (1962).png" alt=""><figcaption></figcaption></figure>

## 서버 명령 생성&#x20;

다음은 할 일 메시지의 자동 팝업을 예로 들어 서버 측 알림을 만들고 적용하는 일반적인 작업 단계를 소개합니다.

> **업무 배경: 직원이 상급자에게 휴가 신청 절차를 제출할 때, 그는 휴가 신청 절차에 대한 새로운 알림이 상사의 현재 실행 중인 페이지에 자동으로 팝업되기를 희망합니다.알림 메시지를 클릭하면 자동으로 로 이동합니다. - 사이트에서 알림 기능을 구현하는 페이지입니다.**

**단계**

![](https://help.grapecity.com.cn/download/thumbnails/80947531/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1673923188000\&api=v2)  개체 관리자에서 서버 알림의 레이블을 마우스 오른쪽 버튼으로 클릭하고 "서버 알림 생성"을 선택하면 서버 알림 생성 대화 상자가 팝업됩니다.

또는 "폴더 만들기"를 선택하여 폴더에 서버 명령을 만듭니다.

<figure><img src="../../../../.gitbook/assets/image (594).png" alt=""><figcaption></figcaption></figure>

리본의 메뉴 모음에서 만들기를 클릭하고 서버 알림 영역에서 서버 알림을 클릭하여 서버 알림을 만들기 위한 대화 상자를 표시할 수도 있습니다.

<figure><img src="../../../../.gitbook/assets/image (1022).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947531/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1673923188000\&api=v2)  서버 쪽 알림에 대한 일반 설정을 편집합니다. 예를 들어 알림 이름을 "프로세스  메시지 알림 남기기"  로설정합니다.

<figure><img src="../../../../.gitbook/assets/image (814).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947531/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1673923188000\&api=v2)  서버 알림의 매개변수를 편집합니다. 매개변수 탭을 클릭하여 매개변수를 추가합니다.

<figure><img src="../../../../.gitbook/assets/image (1088).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947531/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1673923188000\&api=v2)  서버 명령을 생성하면 서버 알림 범주 아래에서 새 서버 알림 명령을 볼 수 있습니다.

<figure><img src="../../../../.gitbook/assets/image (1069).png" alt=""><figcaption></figcaption></figure>

예를 들어 "서버 알림"이라는 서버 명령을 만들고 "수신자" 매개변수를 추가합니다. 명령은 "서버 알림 명령 보내기"입니다. 여기서 이름은 서버 알림의 이름입니다. 여기서는 이전 단계에서 만든 서비스를 선택합니다.

<figure><img src="../../../../.gitbook/assets/image (606).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947531/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1673923188000\&api=v2)  설정이 완료되면 클라이언트(브라우저)에서 이 서버 명령을 호출 할 수 있습니다. 포건시는 클라이언트 단에서 "서버알림"을 제공하며 이 명령을 사용하여 적극적으로 메시지를 푸시할 수 있습니다. 마스터 페이지의 페이지 로딩 명령에 "구독 알림 명령 " 을 넣는 것을 권장합니다 .

<figure><img src="../../../../.gitbook/assets/image (914).png" alt=""><figcaption></figcaption></figure>

"구독 알림 명령 " 뒤에 아래 그림과 같이 "메시지보여주기" 명령과 "페이지 보여주기" 명령을 추가합니다.

<figure><img src="../../../../.gitbook/assets/image (1068).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947531/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1673923188000\&api=v2)  휴가 워크플로우우를 열고 프로세스 속성의  명령을 "서버 명령 호출"로 설정하고 서버 명령 "서버단명령1"을 ​​호출하고 매개 변수를 설정하십시오..

<figure><img src="../../../../.gitbook/assets/image (1021).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947531/%E6%AD%A5%E9%AA%A47.png?version=1\&modificationDate=1673923188000\&api=v2)  프로젝트를 실행하려면 직원 및 감독자 사용자로 각각 로그인하십시오. 직원이 휴가 워크플로우를 시작한 후 관리자는 페이지에 알림 메시지를 받게 되며 "확인"을 클릭하면 할 일 페이지로 이동합니다.
