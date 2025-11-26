# 보고서 데이터 소스 만들기

보고서를 만들기 전에 보고서에 필요한 데이터 소스를 준비해야 합니다. 대상 테이블, 뷰 또는 JSON 데이터 원본을 지정하여 보고서 데이터 원본을 만듭니다.

데이터 소스를 만들면 보고서에 대한 데이터 세트가 자동으로 생성됩니다.

### 보고서 데이터 소스 만들기 <a href="#chuang-jian-bao-biao-shu-ju-yuan" id="chuang-jian-bao-biao-shu-ju-yuan"></a>

**1.** 리포트를 선택하고 마우스 오른쪽 버튼을 클릭한 후, 오른쪽 클릭 메뉴에서 "데이터 소스 생성"을 선택합니다.

<figure><img src="../../.gitbook/assets/image (187).png" alt=""><figcaption></figcaption></figure>

**2.** 데이터소스 생성 대화상자가 나타납니다.

<figure><img src="../../.gitbook/assets/image (188).png" alt=""><figcaption><p><br></p></figcaption></figure>

**3.** 데이터 소스를 구성합니다.

<figure><img src="../../.gitbook/assets/image (189).png" alt=""><figcaption></figcaption></figure>

데이터 소스 유형은 데이터 테이블 또는 JSON 데이터 소스일 수 있습니다.

선택 유형이 데이터 테이블인 경우:

* 이름: 데이터 소스의 이름입니다.
* 테이블: 데이터의 소스 데이터 테이블을 선택합니다.
* 데이터소스 파라미터  수정: 추가된 데이터소스 매개변수는 쿼리 조건, 쿼리 행 번호 등에 사용할 수 있습니다.
* 선택: 데이터 테이블을 선택하면 기본적으로 데이터 테이블의 모든 필드가 선택 목록에 자동으로 추가됩니다. 필요에 따라 열을 추가하거나 제거할 수 있습니다.
* 쿼리 : 데이터 테이블의 데이터에 대한 쿼리 조건을 설정합니다.
* 상위제: 데이터 테이블의 데이터에 대한 쿼리 행 수를 설정합니다.
* 정렬: 데이터 테이블의 데이터에 대한 정렬 규칙을 설정합니다.

유형을 JSON 데이터 소스로 선택하는 경우:

* 이름: 데이터 소스의 이름입니다.
* 템플릿 JSON 설정: 주어진 샘플 JSON 데이터를 구문 분석하여 해당 속성 이름을 가져오고 속성 이름에 따라 열 이름을 설정합니다.

<figure><img src="../../.gitbook/assets/image (190).png" alt=""><figcaption></figcaption></figure>

* 열 추가/제거: 템플릿 JSON을 설정한 후 기본적으로 JSON의 모든 속성이 속성 이름 목록에 자동으로 추가됩니다. 필요에 따라 속성을 추가하거나 제거할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (191).png" alt=""><figcaption></figcaption></figure>

### 데이터세트의 계산된 필드 <a href="#shu-ju-ji-zhong-de-ji-suan-zi-duan" id="shu-ju-ji-zhong-de-ji-suan-zi-duan"></a>

보고서 데이터 소스에서 자동으로 생성된 데이터 세트에 계산된 필드가 있습니다.

<figure><img src="../../.gitbook/assets/image (192).png" alt=""><figcaption></figcaption></figure>

이 필드는 보고서 수식을 필드 계산으로 사용할 수 있으며 해당 기능은 이동형 데이터 테이블의 수식 필드와 거의 동일합니다.

그러나 계산된 필드는 프로그래밍 방식으로 처리되므로 데이터베이스에서 처리되는 수식 필드에 비해 성능이 떨어집니다. 따라서 이동형 데이터 테이블에서는 수식 필드를 사용하는 것이 좋습니다.

자세한 내용은 [수식 필드](../../database/fieldtype/formula.md)를 참조하세요 .

