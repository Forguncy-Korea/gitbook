# modifyTablesData 메서드

### 매서드&#x20;

Forguncy.modifyTablesData(modifyData, callback, errorCallback)

### 설명&#x20;

데이터 테이블의 데이터를 추가/수정/삭제합니다.

이 방법은 다음 두 가지 문제를 해결하는 데 사용됩니다.

1. 현재 포건시는 한 줄의 데이터에 대한 추가 및 삭제를 제공합니다. 그러나 사용자가 동시에 1000개의 행을 추가 또는 삭제하려는 경우 서버에 1,000개의 요청을 보내야 하며, 이는 시간이 오래 걸리고 서버 리소스를 많이 소비합니다.
2. 사용자가 한 번에 1000개의 행을 추가하려는 경우 사용자는 1000개의 행을 반복해야 하지만 한 번 실패하면 이전에 삽입한 데이터를 취소할 수 없습니다. 경우에 따라 모든 삽입을 취소하는 것이 좋습니다.

### 매개변수&#x20;

| 매개변수          | 형식          | 설명                                                                          |
| ------------- | ----------- | --------------------------------------------------------------------------- |
| callBack      | function    | 전자 메일이 성공적으로 전송된 후 호출되는 콜백 함수가 성공했습니다. 이 매개 변수는 선택 사항입니다.                   |
| errorCallback | function    | 전자 메일 전송이 실패한 후 호출되고 매개 변수를 통해 오류 메시지를 알리는 실패한 콜백 함수입니다. 이 매개 변수는 선택 사항입니다. |
| modifyData    | plainObject | 어떤 테이블에 대한 데이터, 추가/수정/삭제된 행 및 열에 대한 데이터를 포함하는 개체를 지정합니다.                    |

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

각각 ID, 이름 및 부서 열이 세 개인 테이블인 테이블 1과 테이블2가 있다고 가정합니다.

1. 여러행의 데이터를 삽입&#x20;

```javascript
// 테이블 1과 테이블 2에 데이터의 여러 행을 삽입합니다.
Forguncy.modifyTablesData({
    테이블1: {
        addRows: [
        {
            이름: "이은지",
            부서: "개",
        },
        {
            이름: "한지",
            부서: "관리부서",
        },
        ]
    },
    테이블2: {
        addRows: [
        {
            이름: "정신",
            부서: "마케",
        },
        {
            이름: "이사",
            부서: "마케",
        },
        ]
    }
});
```

2\. 여려 행의 데이터를 삭제&#x20;

```javascript
// 행 삭제 
Forguncy.modifyTablesData({
    테이블1: {
        deleteRows: [
        {
            ID: 2
        },
        {
            ID: 3
        },
        ]
    },
    테이블2: {
        deleteRows:  [
        {
            ID: 3
        },
        {
            ID: 4
        },
        ]
    }
});
```

3\. **여러 행의 데이터를 업데이트합니다**

```javascript
// 행 업데이트 
Forguncy.modifyTablesData({
    테이블1: {
        editRows: [
        {
            primaryKey:
        {
            ID: 2
        },
        values: {
            이: "한가",
            부: "디자인부서"
        }
        },
        {
        primaryKey:
        {
            ID: 3
        },
        values: {
            이: "이미",
            부: "개발부서"
        }
        },
        ]
    },
    테이블2: {
        editRows: [
        {
        primaryKey:
        {
            ID: 3
        },
        values: {
            姓名: "이자",
            部门: "개발부서"
        }
        },
        {
        primaryKey:
        {
            ID: 4
        },
        values: {
            이: "양주은" ,
            부서: "관리부서"
        }
        },
        ]
    }
});
```

**4. 여러 행의 데이터를 동시에 추가, 삭제 및 수정합니다**

```javascript
// 행 추가, 수정, 삭제
Forguncy.modifyTablesData({
    직원 테이블: {
    addRows: [
    {
    이름: "왕밍",
    부서: "개발",
    },
    {
    이름: "자오 레이",
    부서: "관리 부서",
    },
    ],
    deleteRows: [
    {
    ID: 1
    },
    {
    ID: 2
    },
    ],
    editRows: [
    {
    primaryKey:
    {
    ID: 3
    },
    values: {
    이름: "리틀 리",
    부서: "개발 부서"
    }
    },
    {
    primaryKey:
    {
    ID: 4
    },
    values: {
    이름: "리틀 킹",
    부서: "관리 부서"a
    }
    },
    ]
    }
});
```

{% hint style="info" %}
\[옵션-> 응용 프로그램 실행]에서 "JavaScript Api를 사용하여 데이터베이스에 접근하여 내용을 변경할 수 없습니다." 선택하면 이 메서드를 사용하여 지정된 데이터 테이블에 데이터를 추가할 때 실패합니다. 이 메서드를 사용 하 여이 메서드를 사용 하 여이 작업을 수행 하기 전에이 옵션을 선택 취소 합니다.

![](<../../../../.gitbook/assets/image (2181).png>)
{% endhint %}

### 사용 예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364778/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092720000\&api=v2) 페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72364778/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092720000\&api=v2) 페이지에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

여기서 코드는 여러 줄의 데이터를 추가, 삭제 및 수정하는 샘플 코드 입니다.

<figure><img src="../../../../.gitbook/assets/image (667).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364778/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092720000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 데이터 편집 버튼을 클릭하면 데이터 테이블의 데이터가 추가/삭제됩니다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (754).png" alt=""><figcaption></figcaption></figure>
