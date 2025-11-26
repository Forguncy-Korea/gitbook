# ConvertToCssColor 메서드

### 매서드&#x20;

Forguncy.ConvertToCssColor(color)

### 설명&#x20;

지정된 색상 텍스트를 CSS 색상 텍스트, 즉 색상의 16진수 값으로 변환합니다.

### 매개변수&#x20;



<table><thead><tr><th width="157.33333333333331">매개변수 </th><th width="164">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>color</td><td>string</td><td><p>색상의 텍스트(예: [Background 2 -25 50]와 같은 문자열은 색상이 [배경색 2, 어두운 25%, 투명도 50%]를 나타냅니다.</p><p>문자열은 색상 이름, 색상의 선명도 및 색상의 투명도의 세 부분으로 나뉩니다.</p><ul><li>색상 이름: 색상의 텍스트 문자열에서 이름은 영어로 되어 있습니다. 색상 위로 마우스를 가져가면 색상 이름을 가져올 수 있습니다. </li><li>색상의 밝기: 음수로 표시되고 음수로 음수로 표시된 어둡고 밝은 색상으로 나뉩니다. 예를 들어 60 및 -60, 60은 기본 색상에서 60% 감소를 나타내고 -60은 기본 색상에 60% 더 깊은 색상을 나타냅니다.</li><li>색상이 성격 색상 2이고 색조가 60%인 경우 문자열은 "Accent 2 60"이어야 합니다.</li><li>색상이 성격 색상 2이고 어두운 색상이 60%인 경우 문자열은 "Accent 2 -60"이어야 합니다.</li><li>색상의 투명도: 색상의 투명도를 나타냅니다. 이 매개 변수는 선택 사항이며 설정되지 않은 경우 기본값은 255입니다. 투명도의 범위는 0 ~255입니다.</li></ul></td></tr></tbody></table>

### 반환값&#x20;

string

### 예제&#x20;

다음 예제 코드에서는 ConvertToCssColor 메서드를 통해 지정된 색상 텍스트를 CSS 색상 텍스트로 변환합니다.

```
// 지정된 색상을 변환
var color = Forguncy.ConvertToCssColor("Accent 2 3");
// 변환된 CSS 색상을 보여주는 경고 상자 팝업
alert(color);
```

### 사용예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364541/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092717000\&api=v2) 페이지에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (1715).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364541/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092717000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 색상 변환 버튼을 클릭하면 변환된 CSS 색상( 색상의 16진수 값)을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (562).png" alt=""><figcaption></figcaption></figure>
