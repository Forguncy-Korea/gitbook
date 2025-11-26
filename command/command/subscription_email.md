# 알림 명령 - 이메일 알림 설정 생성하기

이메일 알림 설정 생성하기에서 모니터링되는 테이블과 필드는 물론 메일의 제목과 내용을 설정할 수 있습니다. 데이터 테이블의 데이터가 변경되면 이동식 그리드는 자동으로 이메일을 보내 사용자에게 알릴 수 있습니다.

<figure><img src="../../.gitbook/assets/image (809).png" alt=""><figcaption></figcaption></figure>

## 이메일 알림 설정 생성하기 명령 설정&#x20;

메일 구독 기능을 사용하기 위해서는 먼저 메일 서버를 설정해야 합니다. 자세한 내용은 [메일 서버 구성](../../forguncyserver/serversetting/mailserver.md)을 참조하십시오 .

| 설정         | 설명                                                                                                                                                                                                                    |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 등록된 보기 이름  | 이메일 알림의 제목을 설정합니다.                                                                                                                                                                                                    |
| 대상 테이블     | <p>데이터 테이블이 변경될 때 이메일 알림을 보내도록 선택하십시오.</p><p>"조건 설정"을 체크한 후 조건을 추가하고 이메일 알림을 보내기 위한 조건을 설정할 수 있습니다.</p>                                                                                                               |
| 뷰의 열       | <p>모니터링되는 열, 이러한 필드의 변경 정보도 이메일의 내용이 됩니다. 새 필드를 클릭하여 알림 필드를 추가합니다.</p><ul><li>열: 모니터링되는 필드이며 이 필드의 변경 정보도 이메일의 내용이 됩니다.</li><li>열 표시 이름: 이메일 알림에서 해당 필드의 별칭입니다.</li><li>제목으로 표시: 선택한 필드가 이메일 알림의 제목에 추가됩니다.</li></ul> |
| 고급 설정      | "고급 설정 표시"를 클릭하면 이메일 구성 옵션이 나타나고 발신자 주소, 발신자 이름 및 이메일 헤더 접두사를 설정할 수 있습니다.                                                                                                                                             |



예를 들어 직원목록에서 직원 상태가 변경되면 이메일 알람이 전송됩니다.&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72354420/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092563000\&api=v2)  페이지에 버튼을 추가하고 명령을 "이메일 알림 설정 명령"으로 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72354420/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092563000\&api=v2)  구독 정보를 설정합니다. 이메일 구독의 이름은 "주문정보", 대상 테이블은 "주문정보테이블", "뷰쿼리설정"을 체크하고 "새 조건"을 클릭하고 조건은 "주문 상태"가 "미주문"과 같습니다로.설정합니다.&#x20;

아래 그림에 나와 있습니다.

<figure><img src="../../.gitbook/assets/image (1424).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72354420/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092563000\&api=v2)  알림 필드를 설정합니다. 하나 이상의 알림 필드를 추가하려면 새 필드를 클릭합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72354420/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092563000\&api=v2)  아래 그림과 같이 "고급 설정 표시"를 클릭하여 보낸 사람의 주소, 이름 및 이메일 헤더 접두사를 설정합니다.

<figure><img src="../../.gitbook/assets/image (1773).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72354420/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092563000\&api=v2)  설정이 완료되면 "확인"을 클릭하여 명령 창을 닫습니다.

프로젝트를 실행한 후 "메일 구독" 버튼을 클릭하면 내장된 "이메일 구독" 페이지로 페이지가 이동합니다. 필요에 따라 이메일을 구독하고 확인을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1085).png" alt=""><figcaption></figcaption></figure>

구독 필드가 변경되면 현재 로그인한 사용자가 설정한 사서함으로 해당 메일을 수신할 수 있습니다.
