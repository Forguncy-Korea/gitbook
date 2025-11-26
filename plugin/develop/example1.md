# 포건시 플러그인 예제- 자료형 소개

## 포건시 플러그인에 자료형 소개&#x20;

포건시 플러그인은 별도의 C# 프로그램이므로, C#에서 지원하는 여러가지 자료형(이후 DataType)을 사용할 수 있습니다. 플러그인 API 제작 시 DataType 속성을 정의하시면 설정하신 내용에 따라 적절한 편집기가 기본적으로 생성되며, 설정하신 값이 표시됩니다.

<table><thead><tr><th width="224.33333333333331">자료형</th><th width="226">포건시 편집기</th><th>설명</th></tr></thead><tbody><tr><td>string</td><td>텍스트 에디터</td><td>텍스트 입력 상자, 워터 마크 등</td></tr><tr><td>int</td><td>int 입력 편집기</td><td>정수만 입력 가능한 편집기 사용</td></tr><tr><td>bool</td><td>체크 박스</td><td>체크 박스 모양의 확인 상자 사용</td></tr><tr><td>double</td><td>double 입력 편집기</td><td>소수까지 입력 가능한 편집기 사용</td></tr><tr><td>enum</td><td>콤보 박스</td><td>드롭다운 형식의 콤보 박스 사용</td></tr><tr><td>timespan</td><td>시간 편집기</td><td>시간 셀 유형을 사용</td></tr><tr><td>imagevalue</td><td>그림 편집기</td><td>사용자의 PC를 탐색하여 선택하는 선택창 사용</td></tr><tr><td>list&#x3C;command></td><td>명령 편집기</td><td>버튼에서 명령 편집하여 사용</td></tr></tbody></table>

## DataType 테스트 플러그인 만들기 <a href="#datatype" id="datatype"></a>

1. [포건시 플러그인 생성 도구 다운로드](https://forguncy-korea.github.io/attached_files/Plugin_Files/etc/PluginTools_20200710.zip)하신 뒤 압축을 풀고, ForguncyPluginCreator.exe를 실행하십시오.<br>
2. 프로젝트 이름(Project Name)은 ‘LayDateCellType’으로 정의하시고, 플러그인 유형(PluginType)은 ‘셀 유형(CellType)’, 출력 경로(Output Path)는 플러그인을 작업하실 경로로 입력해 주십시오.

<figure><img src="../../.gitbook/assets/image (2328).png" alt=""><figcaption></figcaption></figure>

3. 플러그인 개발 환경을 생성하신 위치에서 .csproj 파일을 더블 클릭하시면 Visual Studio에서 프로젝트가 열립니다.

<figure><img src="../../.gitbook/assets/image (2329).png" alt=""><figcaption></figcaption></figure>

4. 솔루션 탐색기(Solution Explorer)에서 “참고”를 확장하신 후, 나타나는 Forguncy.CellTypes 및 Forguncy.PluginCommon을 제거하십시오.

<figure><img src="../../.gitbook/assets/image (2330).png" alt=""><figcaption></figcaption></figure>

5. 다시 솔루션 탐색기의 “참조”에서 마우스 오른쪽 클릭하여 “참조 추가(Add Reference)”를 선택하십시오.

<figure><img src="/broken/files/0bG6y4u3VqMWbk5z1J9L" alt=""><figcaption></figcaption></figure>

6. “참조 추가”창의 하단에 있는 “찾아보기(Browse…)”을 클릭하신 후, 포건시 설치 폴더의 Website\bin 폴더로 이동하십시오. 예를 들면, C:\Program Files (x86)\Forguncy\Website\bin 입니다.

<figure><img src="../../.gitbook/assets/image (2331).png" alt=""><figcaption></figcaption></figure>

7. 포건시 설치 위치에서 3개의 라이브러리 파일 GrapeCity.Forguncy.Plugin.dll, GrapeCity.Forguncy.CellTypes.dll, Forguncy.Commands.dll을 찾아 솔루션 탐색기에 추가하십시오.

<figure><img src="../../.gitbook/assets/image (2332).png" alt=""><figcaption></figcaption></figure>

8. 해당 라이브러리 파일들을 추가하시려면 화면에서 OK를 눌러 진행하십시오.

<figure><img src="../../.gitbook/assets/image (2333).png" alt=""><figcaption></figcaption></figure>

9. 파일 3개를 추가한 솔루션 탐색기의 모습은 다음과 같습니다.

<figure><img src="../../.gitbook/assets/image (2334).png" alt=""><figcaption></figcaption></figure>

10. ForguncyPluginDataTypeTest.cs을 열어 상단의 using 부분을 확인합니다. 포건시에서 가져온 파일을 가져오면 아래 그림과 같이 자동으로 등록이 됩니다. 이번 플러그인을 위해서 GrapeCity.Forguncy.Commands를 추가하고 진행하겠습니다.

<figure><img src="../../.gitbook/assets/image (2335).png" alt=""><figcaption></figcaption></figure>

11. ForguncyPluginDataTypeTest.cs를 열어 아래와 같이 편집합니다.

```
//포건시 셀유형 선택 시 왼쪽에 표시할 아이콘의 모양을 정의하는 부분입니다.
[Icon("pack://application:,,,/ForguncyPluginDataTypeTest;component/Resources/Icon.png")]
public class DemoCellType : CellType
{
    //포건시 셀유형 선택 목록에 표시되는 이름을 정의합니다.
    public override string ToString()
    {
        return "포건시 플러그인 자료형 예제"; 
    }

    //포건시 플러그인 DataType 중 String을 이용합니다.
    public string MyStringProperty
    {
        get; set;
    }

    //포건시 플러그인 DataType 중 int를 이용합니다.
    public int MyIntProperty
    {
        get; set;
    }

    //포건시 플러그인 DataType 중 boolean을 이용합니다.
    public bool MyBoolProperty
    {
        get; set;
    }

    //포건시 플러그인 DataType 중 double을 이용합니다.
    public double MyDoubleProperty
    {
        get; set;
    }

    //포건시 플러그인 DataType 중 enum을 이용합니다.
    public MyEnum MyEnumProperty
    {
        get; set;
    }

    //포건시 플러그인 DataType 중 timespan을 이용합니다.
    public TimeSpan MyTimeSpanProperty
    {
        get; set;
    }

    //포건시 플러그인 DataType 중 image value를 이용합니다.
    public ImageValue MyImageProperty
    {
        get; set;
    }

    //포건시 플러그인 DataType 중 command list를 이용합니다.
    public List<Command> MyCommandListProperty
    {
        get; set;
    }
}

//위에서 선언한 enum 관련 표시할 값을 정합니다.
public enum MyEnum
{
    EnumValue1,
    EnumValue2,
    EnumValue3
}
```

12. 이대로 실행해도 되지만, 조금 더 알아보기 쉽도록 아이콘을 변경해 보겠습니다. 먼저, 솔루션 탐색기에서 Icon.png와 PluginLogo.png를 삭제 합니다.

<figure><img src="../../.gitbook/assets/image (2336).png" alt=""><figcaption></figcaption></figure>

13. Icon은 [ForguncyPluginDataTypeIcon.png](https://forguncy-korea.github.io/attached_files/Plugin_Files/V6_ForguncyPluginDataType/ForguncyPluginDataTypeIcon.png)를 다운로드 하셔서 솔루션 탐색기 Resources에 넣으십시오.

<figure><img src="../../.gitbook/assets/image (2337).png" alt=""><figcaption></figcaption></figure>

* 참고 : 아이콘의 크기는 16x16이어야 합니다.
* 이후 하단의 속성(Properties)에서 빌드 설정을 Resource로 설정해 줍니다.

14. ForguncyPluginDataTypeTest.cs를 열어 Icon 정의 부분의 파일명을 업데이트한 파일명과 동일하게 변경합니다.

<figure><img src="../../.gitbook/assets/image (2338).png" alt=""><figcaption></figcaption></figure>

15. 같은 방식으로 Logo로 쓰일 이미지 [ForguncyPluginDataTypePluginLogo.png](https://forguncy-korea.github.io/attached_files/Plugin_Files/V6_ForguncyPluginDataType/ForguncyPluginDataTypePluginLogo.png)를 다운로드 하셔서 솔루션 탐색기 Resources에 넣으십시오.

<figure><img src="../../.gitbook/assets/image (2339).png" alt=""><figcaption></figcaption></figure>

* 참고 : 권장 ThumbNail의 크기는 100x100입니다.
* 이후 하단의 속성(Properties)에서 출력 결과물을 항상 복사(Copy Always)로 설정해 줍니다.

16. PluginConfig.json 파일을 열고 아래와 같이 Image 파일의 이름, Description, Name을 변경합니다.

<figure><img src="../../.gitbook/assets/image (2340).png" alt=""><figcaption></figcaption></figure>

17. 솔루션 탐색기에서 플러그인 이름을 마우스 오른쪽으로 클릭하신 후 “빌드(Build)”합니다.

<figure><img src="../../.gitbook/assets/image (2341).png" alt=""><figcaption></figcaption></figure>

아래와 같이 빌드의 결과가 나타나면, 해당 위치로 이동하십시오.

<figure><img src="../../.gitbook/assets/image (2342).png" alt=""><figcaption></figcaption></figure>

빌드 결과물이 나온 위치에 아래 그림과 같이 zip 파일이 나타납니다. 해당 파일을 따로 복사해서 특정 폴더에 모으셔도 되고, 해당 위치에 두셔도 됩니다.

<figure><img src="../../.gitbook/assets/image (2343).png" alt=""><figcaption></figcaption></figure>

## 포건시에서 DataType 플러그인 사용하기 <a href="#datatype" id="datatype"></a>

1. 포건시를 실행하시고 「파일 > 플러그인」으로 이동하셔서 “플러그인 설치”를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2344).png" alt=""><figcaption></figcaption></figure>

빌드 결과물이 나온 위치에 생성된 zip 파일을 불러옵니다.아래와 같이 플러그인 폴더에 추가되면 성공입니다.

<figure><img src="../../.gitbook/assets/image (2345).png" alt=""><figcaption></figcaption></figure>

2. 다음은 생성한 플러그인을 활용하는 방법입니다.

<figure><img src="../../.gitbook/assets/image (2346).png" alt=""><figcaption></figcaption></figure>

위 프로젝트를 간략히 설명하면 다음과 같습니다.&#x20;

① 통합 셀을 하나 생성합니다.&#x20;

② 샐유형 선택 목록에서 “포건시 플러그인 자료형 예제” 를 선택합니다.

③ 오른쪽 패널에 나타나는 DataType별 UI Control을 확인합니다.

3. 위에서 설명드린 내용은 여기 [▶포건시 플러그인 자료형 테스트 소스코드](https://forguncy-korea.github.io/attached_files/Plugin_Files/V6_ForguncyPluginDataType/ForguncyPluginDataTypeTest_SourceCode.zip)를 클릭하셔서 다운로드 후 Microsoft Visual Studio에서 열어 작업하실 수 있습니다.
