# 바코드

셀을 바코드 유형으로 설정하고 바코드 유형을 QR 코드 또는 1차원 코드로 선택합니다.

<figure><img src="../../.gitbook/assets/image (833).png" alt=""><figcaption></figcaption></figure>

## 바코드 설정&#x20;

바코드를 선택하고 속성 설정 영역에서 셀 설정 탭을 선택하여 바코드 유형을 설정합니다.

바코드 유형에는 QRCode, NW7, Code39, GS1-128, EAN128, CODE128, JAN13이있습니다. QRCode는 7차원코드이고, NW7, Code39, GS1-128, EAN128, CODE128, JAN13은 1차원 코드입니다.

* 바코드 유형에서 QRCode를 선택하는 경우 검사 비트, 버전 및 구조 링크를 생성할지 여부를 설정해야 합니다.
* 바코드 유형이 QRCode 이외의 유형을 선택하는 경우 검사 비트를 생성할지 여부를 설정해야 하며 NW7은 검사 비트 알고리즘을 설정해야 합니다.

바코드 유형을 GS1-128로 선택한 경우 제어 문자 FNC1, FNC2, FNC3, FNC4를 나타내기 위해 %FNC1%, %FNC2%, %FNC2%, %FNC3%, %FNC3%, %FNC4%를 사용합니다.

다음 시나리오에서 GS1-128 바코드 키워드를 사용할 수 있습니다.

* 바코드 값에서 직접 사용;
* 셀 수식에서 사용되며 연결 문자를 사용하여 바코드 문자의 스티치를 지원합니다.
* 데이터 테이블에서 사용됩니다.

<figure><img src="../../.gitbook/assets/image (2283).png" alt=""><figcaption><p>QR코드 </p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (870).png" alt=""><figcaption></figcaption></figure>

