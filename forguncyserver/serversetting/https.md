# Https 인증서

앱을 Https 앱으로 게시하거나 서버관리자를 Https 웹 사이트로 설정해야 하는 경우 Https를 미리 설정하여 포트 바인딩 인증서를 지정해야 합니다. HTTPS는 전문 인증 기관에서 배포한 서버 인증서가 필요합니다.

포건시는 pfx/p12 인증서만 지원합니다. 인증서가 다른 유형인 경우 pfx/p12 인증서로 변환할 수 있습니다.

## Https 인증서 설정&#x20;

Https를 사용하기 전에 Https 인증서 설정이 필요합니다.

**절차를 따르십시오**

![](https://help.grapecity.com.cn/download/thumbnails/72363358/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092700000\&api=v2) 서버관리자에서 설정->Https 인증서를 선택합니다.

![](<../../.gitbook/assets/image (795).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72363358/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092700000\&api=v2) Https 인증서의 쿼리 포트 영역에서 포트 번호를 입력하고 쿼리를 클릭하여 포트에 바인딩된 인증서 정보를 가져옵니다. 기본 포트 번호는 443입니다.

SSL 인증서 정보 영역에서 "인증서 해제"를 클릭하여 현재 포트에서 인증서를 제거합니다. 인증서 목록 보기를 클릭하여 목록 대화 상자를 열고 인증서를 선택한 후 바인딩을 클릭하여 인증서를 현재 포트에 바인합니다.

![](<../../.gitbook/assets/image (684).png>)
