# Echart

ECharts 플러그인은 포건시에 대한 직관적이고 대화형 차트 표시 기능을 제공하는 강력한 데이터 시각화 차트도구입니다. 이 플러그인을 통해 사용자는 라인 차트, 막대 차트, 파이 차트 등 다양한 유형의 차트를 쉽게 생성하여 데이터를 표시하고 분석할 수 있습니다.

포건시는 내부적으로 차트를 지원하지만 사용자들이 사용하면서 이러한 차트 유형이 충분하지 않다고 느끼고 더 많은 차트 유형을 지원하기를 희망하는 경우가 많습니다. 이  문제를 해결하기 위해 ECharts 플러그인이 추가되었습니다.

하지만  Echart플러그인은  약간의 코드를 이해하고 작성해야 한다는 것입니다. 결국 ECharts 에는 많은 설정이 있고 다양한 차트의 구성이 다르기 때문에 인터페이스를 노출하는 것이 가장 좋은 방법입니다. 하지만 한 가지 안심할 수 있는 것은 포건시에 대해 보편적으로 만들 수 있는 모든 작업을 수행했다는 것입니다.&#x20;



### 플러그인 다운로드

<table><thead><tr><th width="151">버전</th><th>다운로드</th></tr></thead><tbody><tr><td>V10 </td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/EchartsCustomCellType.zip">EchartsCustomCellType.zip</a></td></tr></tbody></table>



### 사용방법&#x20;

1. 페이지 영역을 선택한 후 ECharts 셀을 선택합니다.

<figure><img src="../../../.gitbook/assets/image (270).png" alt=""><figcaption></figcaption></figure>

2. 데이터바인딩을 합니다.&#x20;

데이터바인딩은 데이터테이블의 데이터를 사용하는 경우, JSON Data를 사용하는 경우,

데이터테이블과 JSON Data를 함께 사용하는 경우가 있습니다.&#x20;

1\) 데이터 소스

셀 설정에서 데이터 소스를 직접 선택하고, 데이터 소스 설정에서 데이터 소스명을 생성한 후(영문 이름 권장), 데이터 소스를 설정하여 데이터 테이블을 선택하고, 필요한 필드(데이터)를 선택하면 됩니다.

<figure><img src="../../../.gitbook/assets/image (271).png" alt=""><figcaption></figcaption></figure>

데이터 소스를 선택한 후 \[ECharts Config]을 클릭하여 ECharts 편집 페이지 로 들어갑니다 .

코드를 입력한후 \[Run]버튼을 클릭하면 미리보기에서 차트가 나옵니다.

<figure><img src="../../../.gitbook/assets/image (272).png" alt=""><figcaption></figcaption></figure>

기본적으로 객체를 생성한 후 정의된 데이터 소스(예: DataSource )와 숫자 값(예: Date , SalesData ) 을 설정합니다.



| 기본 코드                                                                                                                                                                                                                                                                                                                                        | 수정된 코드                                                                                                                                                                                                                                                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>option = ｛</p><p>  xAxis: ｛</p><p>    type: 'category',</p><p>    data: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']</p><p>  ｝,</p><p>  yAxis: ｛</p><p>    type: 'value'</p><p>  ｝,</p><p>  series: [</p><p>    ｛</p><p>      data: [150, 230, 224, 218, 135, 147, 260],</p><p>      type: 'line'</p><p>    ｝</p><p>  ]</p><p>｝;</p> | <p>const｛</p><p>  Date:xAxisData,</p><p>  SalesData:yAxisData</p><p>｝ = ForguncyEchartsHelper.splitDataSource(Context.DataSource)</p><p> </p><p>option = ｛</p><p>  xAxis: ｛</p><p>    type: 'category',</p><p>    data: xAxisData</p><p>  ｝,</p><p>  yAxis: ｛</p><p>    type: 'value'</p><p>  ｝,</p><p>  series: [</p><p>    ｛</p><p>      data: yAxisData,</p><p>      type: 'line'</p><p>    ｝</p><p>  ]</p><p>｝;</p> |



### ForguncyEchartsHelper 클래스 설명

```
declare class ForguncyEchartsHelper {
    /**
     * Split object list to multiple list
     * example
     * //splitDataSource basic usage
     * const rawData = [
     *   { date: 'Mon', value: 1 },
     *   { date: 'Tue', value: 2 },
     *   { date: 'Wed', value: 3 },
     *   { date: 'Thu', value: 4 },
     *   { date: 'Fri', value: 5 },
     *   { date: 'Sat', value: 6 },
     *   { date: 'Sun', value: 7 }
     * ]
     * const { date, value } = ForguncyEchartsHelper.splitDataSource(rawData)
     * //date:['Mon','Tue'...]
     * //value:[1,2,3,....]
     * 
     * //splitDataSource with Unique and formatter
     * const rawData = [
     *   { date: 'Mon', value: 1 },
     *   { date: 'Tue', value: 1 },
     *   { date: 'Wed', value: 1 },
     *   { date: 'Thu', value: 1 },
     *   { date: 'Fri', value: 1 },
     *   { date: 'Sat', value: 1 },
     *   { date: 'Sun', value: 1 }
     * ]
     * const { date, value } = ForguncyEchartsHelper.splitDataSource(rawData, {
     *   unique: {
     *     value: true
     *   }, formatter: {
     *     date: (value, index) => 'Day' + (index + 1) + ":" + value
     *   }
     * });
     * //date:['Day1:Mon','Day2:Tue'...]
     * //value:[1]
     */
    public static splitDataSource<T extends { [args: string]: any }>(objList: T[], option?: SplitDataSourceOption): { [args: string]: any[] | undefined }
    /**
     * Group object list by key
     * 
     * //groupBy basic usage
     * const rawData = [
     *   { date: 'Mon', value: 1 },
     *   { date: 'Tue', value: 1 },
     *   { date: 'Tue', value: 2 },
     * ]
     * const res = ForguncyEchartsHelper.groupBy(rawData, { key: 'date' });
     * // {
     * //     "Mon": [
     * //         {
     * //             "date": "Mon",
     * //             "value": 1
     * //         }
     * //     ],
     * //     "Tue": [
     * //         {
     * //             "date": "Tue",
     * //             "value": 1
     * //         },
     * //         {
     * //             "date": "Tue",
     * //             "value": 2
     * //         }
     * //     ]
     * // }
     * 
     * //groupBy with formatter
     * const rawData = [
     *   { date: 'Mon', value: 1 },
     *   { date: 'Tue', value: 1 },
     *   { date: 'Tue', value: 2 },
     * ]
     * const res = ForguncyEchartsHelper.groupBy(rawData, { key: 'date',formatter:(item,index)=>item.value });
     * 
     * // {
     * //     "Mon": [
     * //         1
     * //     ],
     * //     "Tue": [
     * //         1,
     * //         2
     * //     ]
     * // }
     */
    public static groupBy<T extends { [args: string]: any }>(objList: T[], option: GroupByOption<T>): { [args: string]: any[] | undefined }
    /**
     * Convert object list to data set
     * 
     * //toDataSet basic usage
     * 
     * const rawData = [
     *   { date: 'Mon', value: 1 },
     *   { date: 'Tue', value: 1 },
     *   { date: 'Tue', value: 2 },
     * ]
     * const res = ForguncyEchartsHelper.toDataSet(rawData);
     * //res:
     * // [
     * //     [
     * //         "date",
     * //         "value"
     * //     ],
     * //     [
     * //         "Mon",
     * //         1
     * //     ],
     * //     [
     * //         "Tue",
     * //         1
     * //     ],
     * //     [
     * //         "Tue",
     * //         2
     * //     ]
     * // ]
     */
    public static toDataSet<T extends { [args: string]: any }>(objList: T[]): any[];
    /**
     * @param attachment forguncy attachement column value
     * @param index index of attachment file (if you have multiple files)
     */
    public static getAttachment(attachment?: string, index?: number): Promise<Response | undefined>;
    /**
     * @param src forguncy image column value (image src)
     */
    public static getUploadImage(src: string): string
}
/**
 * if set unique true, the same value will be ignored.
 * if set formatter, the value will be formatted.
 */
interface SplitDataSourceOption {
    unique?: { [args: string]: true }
    formatter?: { [args: string]: (value: any, index: number) => any }
}
/**
 * @param key key of object list.
 * formatter can be used to format the value. For example: {date:'Mon',value:1}=>1
 */
interface GroupByOption<T> {
    key: string,
    formatter?: (value: T, index: number) => any
}
```



```
declare namespace Forguncy {
    class Helper {
        public static SpecialPath: SpecialPath;
    }
    class SpecialPath {
        public getUploadImageFolderPathInServer: () => string
        public getFileDownloadUrl: (fileName: string) => string;
    }
    export {
        Helper
    }
}
```



2\) JSON Data Source&#x20;

데이터바인딩에서 JSON 데이터소스를 선택한 후, \[JSON 데이터 소스]를 클릭합니다.

JSON 데이터 소스 창에서 JSON데이터를 아래와 같은 형식으로 입력합니다.

<figure><img src="../../../.gitbook/assets/image (90).png" alt=""><figcaption></figcaption></figure>

ECharts 구성을 클릭하여 아래와 같이 코드를 작성합니다.

<figure><img src="../../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure>

코드 작성 후 실행버튼을 클릭하면 차트 미리보기를 확인할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>



Echarts 에는 많은 고급 구성도 있습니다.

자세한 내용은 [https://echarts.apache.org/zh/option.html#title](https://echarts.apache.org/en/option.html#angleAxis)을 참조하세요.
