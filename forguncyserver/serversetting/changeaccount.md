# 서버 실행 계정 변경

포건시 서버는 기본적으로 실행 계정이 로컬 시스템 계정인 로컬 서비스로 실행됩니다. 대부분의 경우 서비스를 실행하는 계정을 수정할 필요가 없습니다. 그러나 외부 체인 데이터베이스에 액세스할 수 있는 권한이 특정 시스템 계정만 있거나 브라우저에 구성된 에이전트를 사용해야 하는 경우와 같은 경우에 서비스를 실행하는 계정을 수정해야 합니다.

이 섹션에서는 포건시 서버 쪽의 실행 계정을 변경하는 방법에 대해 설명합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72363430/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092701000\&api=v2) Windows 시작 메뉴를 열고 제어판-> 시스템 및 보안-> 관리 도구-> 서비스를 선택하고 목록에서 ForguncyServerService를 찾아 두 번 클릭합니다.

![](<../../.gitbook/assets/image (2131).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72363430/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092701000\&api=v2) 대화 상자에서 로그인 탭을 선택하고 이 계정을 선택하고 데이터베이스에 액세스할 수 있는 사용자 이름과 암호를 입력합니다.

![](<../../.gitbook/assets/image (1149).png>)

{% hint style="info" %}
* 사용자는 관리자여야 합니다.
* 사용자 암호는 비어 있지 않아야 합니다.&#x20;
{% endhint %}

![](https://help.grapecity.com.cn/download/thumbnails/72363430/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092701000\&api=v2) 포건시 서버를 다시 시작합니다. \[ForguncyServerService]를 마우스 오른쪽 버튼 클릭하고 \[다시 시작]을 선택합니다.

![](<../../.gitbook/assets/image (1829).png>)
