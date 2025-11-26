# 바코드





Barcode 컨트롤은 Codabar 및 QR 코드와 같은 다양한 종류의 바코드를 지원합니다.

Barcode 컨트롤은 단독으로 사용할 수도 있고 Table 데이터 영역의 셀에 포함하여 사용할 수도 있습니다.

지원되는 바코드 유형은 다음과 같습니다.



<table><thead><tr><th width="210">바코드 종류</th><th width="356">설명</th><th>샘플</th></tr></thead><tbody><tr><td><strong>ANSI 3 of 9</strong></td><td>알파벳 대문자, 숫자, -, *, $, /, +, %를 사용합니다.</td><td><img src="https://docs.forguncy.com/v10/Media/28/barcode-ansi39.png" alt=""></td></tr><tr><td><strong>ANSI Extended 3 of 9</strong></td><td>전체 ASCII 문자 집합을 사용합니다.</td><td><img src="https://docs.forguncy.com/v10/Media/28/barcode-ansi39x.png" alt=""></td></tr><tr><td><strong>Codabar</strong></td><td>A, B, C, D, +, -,:, ., /, $, 숫자를 사용합니다.</td><td><img src="../../../.gitbook/assets/image (51).png" alt="" data-size="original"></td></tr><tr><td>Code 128 A</td><td>제어 문자, 숫자, 기호, 알파벳 대문자를 사용합니다.</td><td><img src="../../../.gitbook/assets/image (52).png" alt="" data-size="original"></td></tr><tr><td><strong>Code 128 B</strong></td><td>기호, 숫자, 알파벳 대문자, 소문자를 사용합니다.</td><td><img src="../../../.gitbook/assets/image (53).png" alt="" data-size="original"></td></tr><tr><td><strong>Code 128 C</strong></td><td>숫자만 사용합니다.</td><td><img src="../../../.gitbook/assets/image (54).png" alt="" data-size="original"></td></tr><tr><td>Code <strong>128 자동</strong></td><td>전체 ASCII 문자 집합을 사용합니다.</td><td><img src="../../../.gitbook/assets/image (55).png" alt="" data-size="original"></td></tr><tr><td>Code 93</td><td>알파벳 대문자, %, $, *, /, +, -, 숫자를 사용합니다.</td><td><img src="../../../.gitbook/assets/image (56).png" alt="" data-size="original"></td></tr><tr><td><strong>Interleaved 2 of 5</strong></td><td>숫자만 사용합니다.</td><td><img src="../../../.gitbook/assets/image (57).png" alt="" data-size="original"></td></tr><tr><td>Code <strong>39</strong></td><td>숫자, %, *, $, /, ., -, +, 알파벳 대문자를 사용합니다.</td><td><img src="../../../.gitbook/assets/image (58).png" alt="" data-size="original"></td></tr><tr><td><strong>Extended Code 39</strong></td><td>ASCII 문자 세트 전체를 사용합니다.</td><td><img src="../../../.gitbook/assets/image (59).png" alt="" data-size="original"></td></tr><tr><td><strong>Code 49</strong></td><td>8문자씩 2행에서 8행으로 이루어지는 고밀도 스택형 2차원 바코드입니다. 각 행에는 시작 코드와 정지 코드가 있습니다. ASCII 문자 집합 전체를 인코딩합니다.</td><td><img src="../../../.gitbook/assets/image (60).png" alt="" data-size="original"></td></tr><tr><td><strong>Extended Code 93</strong></td><td>ASCII 문자 세트 전체를 사용합니다.</td><td><img src="../../../.gitbook/assets/image (61).png" alt="" data-size="original"></td></tr><tr><td><strong>Data Matrix</strong></td><td>정사각형 또는 직사각형 행렬로 배치된 정사각형 모듈을 포함하는 고밀도 스택형 2차원 바코드입니다.</td><td><img src="../../../.gitbook/assets/image (62).png" alt="" data-size="original"></td></tr><tr><td><strong>EAN-13</strong></td><td>숫자만(12자리 숫자와 체크 디지트)을 사용합니다. 13개의 숫자가 있으면 체크섬을 확인하고 올바르지 않으면 오류를 throw합니다.</td><td><img src="../../../.gitbook/assets/image (63).png" alt="" data-size="original"></td></tr><tr><td><strong>EAN-8</strong></td><td>숫자만(7자리 숫자와 체크 디지트)을 사용합니다.</td><td><img src="../../../.gitbook/assets/image (64).png" alt="" data-size="original"></td></tr><tr><td><strong>GS1 QR Code</strong></td><td><p>QR 코드의 서브 세트이며, 상품 식별 코드(GTIN)와 그 상품에 관한 정보·서비스를 제공하는 Web 사이트의 URL을 표시하는 2차원 심볼입니다.</p><p>따라서, 이 바코드 형식을 사용하는 경우, 상품 식별 코드(GTIN)와 그 상품에 관한 정보등을 제공하는 Web 사이트의 URL이 필요합니다.</p><p>GS1QRCode를 사용하는 것으로, GS1 표준으로 정해진 규격에 준거해, 어플리케이션 식별자를 포함한 정보(GTIN·URL)를 2차원 심볼(QR 코드)에 encode 할 수가 있습니다.</p><p>제한사항: 영숫자만 설정할 수 있습니다.</p></td><td><img src="../../../.gitbook/assets/image (65).png" alt="" data-size="original"></td></tr><tr><td><strong>ITF-14</strong> </td><td>ITF(Interleaved 2 of 5) 타입의 바코드입니다. 표준 물류 바코드로 사용됩니다.</td><td><img src="../../../.gitbook/assets/image (66).png" alt="" data-size="original"></td></tr><tr><td><strong>Japanese Postal</strong></td><td>일본 우편 시스템에서 사용됩니다. 숫자, 하이픈(-), 영문자로 구성된 우편 번호 및 주소 표시 번호를 수용합니다.</td><td><img src="../../../.gitbook/assets/image (67).png" alt="" data-size="original"></td></tr><tr><td><strong>PDF417</strong></td><td><p>가장 많이 사용되는 고밀도 2차원 심볼입니다. 최대 1,108바이트의 정보를 인코딩할 수 있습니다. 이 바코드는 작은 바코드를 쌓아서 구성됩니다. ASCII 문자 집합 전체를 인코딩합니다.</p><p>10개의 오류 수정 레벨과 3가지 데이터 압축 모드(텍스트, 바이트, 숫자)가 있습니다. 이 기호는 1850자의 영숫자 또는 2710자까지 인코딩할 수 있습니다.</p></td><td><img src="../../../.gitbook/assets/image (68).png" alt="" data-size="original"></td></tr><tr><td><strong>QR Code</strong></td><td>숫자, 영숫자, 바이트 데이터, 일본어 한자와 가나 문자를 처리할 수 있는 2차원 심볼입니다. 이 기호는 최대 7366자까지 인코딩할 수 있습니다. 이것이 기본 바코드 스타일입니다.</td><td><img src="../../../.gitbook/assets/image (69).png" alt="" data-size="original"></td></tr><tr><td><strong>RSS-14</strong></td><td>전방향형 POS 스캔용 EAN.UCC 품목 식별을 사용하고 있는 14자리의 공간 절약 심볼입니다. RSS 제품군의 바코드는 GS1 DataBar라고도 합니다.</td><td><img src="../../../.gitbook/assets/image (70).png" alt="" data-size="original"></td></tr><tr><td><strong>RSS-14 Stacked</strong></td><td>RSS14Truncated와 마찬가지로, 인디케이터 디지트를 포함한 EAN.UCC 정보를 사용합니다만, 폭이 좁은 경우는 2단으로 쌓입니다.</td><td><img src="../../../.gitbook/assets/image (71).png" alt="" data-size="original"></td></tr><tr><td><strong>RSS-14 Stacked Omnidirectional</strong></td><td>RSS14와 마찬가지로 전방향 스캔을 포함한 EAN.UCC 정보를 사용하지만 폭이 좁은 경우에는 2단으로 적층됩니다.</td><td><img src="../../../.gitbook/assets/image (72).png" alt="" data-size="original"></td></tr><tr><td><strong>RSS-14 Truncated</strong></td><td>RSS14와 마찬가지로 EAN.UCC 정보를 사용하지만 POS 시스템에서 스캔되지 않은 작은 항목에 사용하기 위해 0 또는 1 표시기 숫자를 포함합니다.</td><td><img src="../../../.gitbook/assets/image (73).png" alt="" data-size="original"></td></tr><tr><td><strong>RSS Limited</strong></td><td>RSS14와 마찬가지로 EAN.UCC 정보를 사용하지만 POS 시스템에서 스캔되지 않은 작은 항목에 사용하기 위해 0 또는 1 표시기 숫자를 포함합니다.</td><td><img src="../../../.gitbook/assets/image (74).png" alt="" data-size="original"></td></tr><tr><td><strong>UCC/EAN-128</strong></td><td><p>GS1-128 표준을 준수합니다. GS1-128은 애플리케이션 식별자 시리즈를 사용하여 데이터를 인코딩합니다. 이 바코드는 ASCII 문자 세트의 모든 문자를 사용합니다.</p><p>또한 이 바코드는 FNC1 문자를 첫 번째 문자 위치로 사용합니다.</p><p>애플리케이션 식별자를 사용하여 만기 날짜, 일괄처리 번호, 가중치 등의 속성을 인코딩할 수 있습니다. 이 바코드는 HIBC 어플리케이션에서도 사용됩니다.</p></td><td><img src="../../../.gitbook/assets/image (75).png" alt="" data-size="original"></td></tr><tr><td><strong>UPC-A</strong></td><td>숫자만(11자리 숫자 및 체크 디지트)을 사용합니다.</td><td><img src="../../../.gitbook/assets/image (76).png" alt="" data-size="original"></td></tr><tr><td><strong>UPC-E0</strong></td><td><p>숫자만 사용합니다. Zero Suppression의 UPC 기호에 사용됩니다.</p><p>Caption 속성에는 6자리 UPC-E 코드 또는 11자리(필수 코드 유형 '0' 포함)의 전체 UPC-A 코드를 입력해야 합니다.</p><p>11자리 코드를 입력하면 Barcorde 컨트롤은 (가능한 경우) 이 코드를 6자리 UPC-E 코드로 변환합니다. 변환할 수 없는 경우에는 아무 것도 표시되지 않습니다.</p></td><td><img src="../../../.gitbook/assets/image (77).png" alt="" data-size="original"></td></tr><tr><td><strong>UPC-E1</strong></td><td>숫자만 사용합니다. 일반적으로 소매점 라벨에 사용됩니다. UPC-E1의 입력 문자열의 길이는 6자리 숫자입니다. E1은 6 영숫자입니다.</td><td><img src="../../../.gitbook/assets/image (78).png" alt="" data-size="original"></td></tr></tbody></table>

이 페이지에서는 Barcode 컨트롤의 기본 설정과 조작 방법을 설명합니다.

1. **도구 상자에서 Barcode를 선택하여 드래그 앤 드롭하거나 클릭하여 디자인 영역에 추가합니다.**

<figure><img src="../../../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure>

2. **전체 Barcode 컨트롤을 선택하고 다양한 속성을 설정합니다.**

실제 사용의 경우에는 \[값] 속성과 \[유형형] 속성의 설정이 필수입니다. 값 속성은 정적 문자열을 설정할 수도 있지만 종종 데이터 연결을 수행하고 사용합니다.

<figure><img src="../../../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

### 표 데이터 영역의 셀에 배치하는 예

1. **Barcode 컨트롤을 Table 데이터 영역의 셀로 드래그 앤 드롭하여 열 너비와 행 높이를 조정합니다.**

<figure><img src="../../../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure>

2. **두 Barcode 컨트롤의 값 속성에 주문 번호 필드를 데이터로 연결합니다.**<br>

<figure><img src="../../../.gitbook/assets/image (82).png" alt=""><figcaption></figcaption></figure>



3. **왼쪽의 Barcode 컨트롤의 \[유형] 속성을 "ANSI 3 of 9"로 설정합니다.**<br>

<figure><img src="../../../.gitbook/assets/image (83).png" alt=""><figcaption></figcaption></figure>



4. **자동 영역 속성을 설정하여 내부 여백을 만듭니다.**<br>

<figure><img src="../../../.gitbook/assets/image (85).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure>

5. **\[캡션 표시 위치] 속성을 설정하고 \[ANSI 3 of 9]에 표시되는 캡션의 위치를 ​​조정합니다**

<figure><img src="../../../.gitbook/assets/image (87).png" alt=""><figcaption></figcaption></figure>

6. 보고서를 미리보고 확인합니다.

<figure><img src="../../../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure>
