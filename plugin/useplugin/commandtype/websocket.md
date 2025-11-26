# WebSocket클라이언트 명령

웹소켓인클라이언트 플러그인을 이용하여 인스턴트 메시지 알림을 받을 수 있습니다.

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/WebSocketClientCommand.zip">WebSocketClientCommand.zip</a></td></tr><tr><td>v 9.0</td><td> <a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/WebSocketClientCommand.zip">WebSocketClientCommand.zip</a></td></tr></tbody></table>

버튼 및 페이지 명령에서 사용이 가능하며, 서버단 명령에서는 사용할 수 없습니다.

<figure><img src="/broken/files/Vn6q3xBPISlB5oCAADJe" alt=""><figcaption></figcaption></figure>

* URL : 웹소켓 URL을 설정합니다.&#x20;
* Sec-WebSocket-Protocol: Sec-WebSocket-Protocol을 설정합니다. 다음과 같이 서버 단에서 이 값을 가져와 사용할 수 있습니다.  &#x20;

```
HttpContext.Request.Headers.TryGetValue("Sec-WebSocket-Protocol", out var protocol); 
            using var webSocket = await HttpContext.WebSockets.AcceptWebSocketAsync(protocol);
```

* 결과를 변수에 저장: websocket 데이터를 변수에 저장하여 후속 명령에서 사용할 수 있습니다.

하위명령 : WebSocket클라이언트 명령의 하위명령을 설정하고 알림을 받을 떄 이 하위 명령을 실행합니다. 예를 들어 하위 명령을 "팝업 메시지 상자" 명령으로 설정합니다.&#x20;
