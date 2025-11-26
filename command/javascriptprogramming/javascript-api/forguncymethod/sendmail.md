# SendMail 메서드

### 매서드&#x20;

Forguncy.SendMail(to, title, content, \[successCallBack], \[failCallBack])

### 설명&#x20;

지정된 이메일 주소로 제목과 콘텐츠를 지정하는 이메일을 보내고 발신자는 현재 웹 사이트에 로그인한 사용자입니다. 이 API를 사용하여 전자 메일을 보내려면 SMTP 서비스를 올바르게 구성해야 합니다. SMTP 서비스 구성은 [메일 서버 구성](../../../../forguncyserver/serversetting/mailserver.md)을 참조하십시오.

{% hint style="info" %}
로그인하지 않은 경우 API를 사용하여 전자 메일을 보낼 수 없습니다.
{% endhint %}

### 매개변수&#x20;



| 매개변수            | 형식                     | 설명                                                                                      |
| --------------- | ---------------------- | --------------------------------------------------------------------------------------- |
| to              | string                 | 받는 사람의 이메일 주소를 지정합니다. 여러 받는 사람인 경우 쉼표로 구분합니다.                                           |
| title           | string                 | 전자 메일 제목입니다.                                                                            |
| content         | string                 | 전자 메일 메시지의 본문 내용을 지정합니다. 일반 텍스트 전자 메일 본문을 사용하는 것 외에도 HTML로 표시된 문자열을 사용할 수 있습니다.         |
| successCallback | function               | 전자 메일이 성공적으로 전송된 후 호출되는 콜백 함수를 지정합니다. 이 매개 변수는 선택 사항입니다.                                |
| failCallback    | function（errorMessage） | 전자 메일 전송이 실패한 후 호출되고 erorMessage 매개 변수를 통해 오류 메시지를 알리는 콜백 함수를 지정합니다. 이 매개 변수는 선택 사항입니다. |

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서 SendMail 메서드를 사용하여 지정 된 전자 메일 주소에 제목 및 콘텐츠를 지정 하는 전자 메일을 보냅니다.

```javascript
// 일반 텍스트 이메일 보내기
Forguncy.SendMail("example1@example.com", "주문 경고 이메일", "최근 주문량이 대폭 증가하여 재고가 소진될 예정입니다. 제 때 처리해 주세요.);
   
// 여러 수신자에게 이메일을 쉼표로 구분하여 보냅니다.
Forguncy.SendMail("example1@example.com,example2@example.com", "주문 경고 메일", "최근 주문량이 크게 증가하여 재고가 소진될 예정입니다. 제때 처리해주세요.);
   
// HTML 형식으로 이메일 보내기
Forguncy.SendMail("example1@example.com", "Order Warning Email", "<h1>Insufficient Inventory Warning</h1><p>최근 주문량이 크게 증가하여 재고가 소진될 예정입니다. 제때 처리해주세요.</p>);
   
// 콜백 함수를 통해 이메일이 성공적으로 전송되었는지 표시
Forguncy.SendMail("example1@example.com", "주문 경고 메일", "최근 주문량이 크게 증가하여 재고가 소진될 예정입니다. 제때 처리해주세요 ",  function () {
//전송에 성공하면 메일이 성공적으로 전송되었다는 경고창이 뜹니다.
alert("이메일이 성공적으로 발송되었습니다.");
 },
//전송이 실패하면 경고 상자가 나타나 오류 메시지를 표시합니다.
function (errorMessage) {
alert(errorMessage);
}
);
```
