# 명령 확인

1. 팝업 데이터 검증 대화상자에서 검증 조건을 "명령"로 설정합니다. 이때 "공백 무시" 옵션은 숨겨집니다.

<figure><img src="../../../.gitbook/assets/image (2402).png" alt=""><figcaption></figcaption></figure>

2. "데이터 검증 명령 설정" 하이퍼링크를 클릭하여 명령 대화 상자를 엽니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (2403).png" alt=""><figcaption></figcaption></figure>

3.  명령 대화 상자에서 다음과 같이 명령을 설정합니다.

    변수 설정 명령을 사용하고, 변수 이름은 len이고, 변수 값은 수식 "=len(D3)"이고, D3은 텍스트 상자가 위치한 셀입니다.

<figure><img src="../../../.gitbook/assets/image (2404).png" alt=""><figcaption></figcaption></figure>

조건부 명령을 사용하여 판단합니다. len 변수의 값이 6보다 크면 "텍스트 상자의 값은 6보다 작거나 같아야 합니다"라는 메시지가 반환됩니다.

<figure><img src="../../../.gitbook/assets/image (2408).png" alt=""><figcaption></figcaption></figure>

유효성을 검사할 값인 데이터 유효성 검사 매개 변수 " 새로운값"을 명령에 사용할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (2405).png" alt=""><figcaption></figcaption></figure>

5. 페이지를 실행하고 텍스트 상자에 "2"를 입력한 후 다른 빈 공간을 클릭하면 오류 메시지가 나타납니다.

<figure><img src="../../../.gitbook/assets/image (2409).png" alt=""><figcaption></figcaption></figure>
