# 보안 설정

포건시에서 모든 앱 및 관리 콘솔 사이트를 설정하는 등 보안 설정을 수행할 수 있습니다.

## 모든 앱의 기본 설정&#x20;

포건시의 서버관리자에서 \[설정-> 웹 보안 설정]을 선택하여 보안 설정 페이지로 이동합니다.

모든 앱의 기본 설정에서 \[포건시 서버 내 모든 애플리케이션에 대한 기본 웹 보안 설정]을 설정하면 관리 콘솔의 모든 앱에 적용됩니다.

![](<../../.gitbook/assets/image (326).png>)

* Http 참조 허용 목록: "referrer" 요청 헤더에서 사용할 수 있는 URL을 구성하고 와일드카드\*를 지원하며 여러 URL 간에 줄 바꿈으로 구분할 수 있습니다.
*   iframe CORS 정책: DENY, SAMEORIGIN 및 ALLOW-FROM의 세 가지 전략이 있습니다.

    * DENY: < iframe > 요소에 사이트를 표시하지 않도록 합니다.
    * SAMEORIGIN: 사이트는 동일한 원본 페이지의 < iframe > 요소에만 표시할 수 있습니다.
    * ALLOW-FROM: 사이트는 지정한 페이지의 < iframe > 요소에만 표시할 수 있습니다. < iframe > 요소에서 사이트를 허용하는 URL을 구성할 수 있습니다.



    <figure><img src="../../.gitbook/assets/image (449).png" alt=""><figcaption></figcaption></figure>

각 앱에 대해 별도의 Http 참조 허용 목록 및 iframe CORS 규칙을 설정할 수도 있습니다. 모든 앱 목록에서 앱을 클릭하여 일반 설정 인터페이스로 이동하여 고급 설정에서 보안 설정을 수행할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (147).png" alt=""><figcaption></figcaption></figure>

## Forguncy 서버 관리자 웹 보안 설정 &#x20;

Http 참조 허용 목록 및 iframe CORS 규칙: 서버관리자의 설정에서 관리 콘솔에 적용되는 Http Referer 허용 목록 및 iframe 도메인 간 정책을 설정합니다.

* 서버관리자 보안 설정: 이 옵션을 선택하면 관리 콘솔이 SSL(보안 소켓 계층)을 사용하여 연결을 암호화합니다.

![](<../../.gitbook/assets/image (563).png>)

## 사용자 서비스 도메인 설정&#x20;

서버 관리자의 도메인 이름을 설정할 수 있으며, 설정된 도메인 이름이 기록되어 암호 검색 하이퍼링크가 포함된 메시지와 같은 일부 필요한 설정에서 사용할 수 있습니다.

이 섹션에서는 서버 관리자의 도메인 이름을 수행하는 방법에 대해 설명합니다.

포건시의 서버관리자에서 설정-> 웹 보안 설정을 선택하여 보안 설정 페이지로 이동합니다.

설정 관리 콘솔 사이트의 도메인 이름 영역에서 텍스트 상자를 클릭하고 텍스트 상자에 설정된 도메인 이름을 입력한 다음 완료되면 설정 저장을 클릭하고 서비스를 다시 시작합니다.

![](<../../.gitbook/assets/image (2281).png>)

### 포건시사이트 세션 설정 <a href="#guan-li-kong-zhi-tai-zhan-dian-hui-hua-de-she-zhi" id="guan-li-kong-zhi-tai-zhan-dian-hui-hua-de-she-zhi"></a>

"세션 활성화"를 선택하면 사용자가 조작하지 않을 때 연결 유지 시간을 설정할 수 있습니다. 기본값은 120분입니다.

이 시간 내에 아무런 조치도 취하지 않으면 세션이 만료되며 관리 콘솔에 다시 로그인해야 합니다. 세션 시간은 2 \~ 1440(분)까지 설정할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (148).png" alt=""><figcaption></figcaption></figure>
