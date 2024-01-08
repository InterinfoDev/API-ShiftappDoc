# apiFilterOption
取得下拉資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiFilterOption
```

### HTTP Request Mehod
```
POST
```

### Request body
| Key | Value | Type | Description |
|:----------|:-------------|:-----|:------------|
| uid | 98599308101484732326 | String | 需透過apiLogin取得
| right | 51341911904173543336756162544864820 | String | 需透過apiLogin取得 |

### JSON representation
Here is a JSON representation of request.
```json
{
  "requestHeader": {
  },
  "requestBody": {
    "companyId": "TW",
    "depNumber": 495,
    "shiftYM": "202306"
  },
  "uid":"98599308101484732326",
  "right":"51341911904173543336756162544864820"
}
```

### Properties
| Property | Type | Description |
|:---------|:-----|:------------|
| requestHeader | Object | 要求本文 |
| requestBody | Object | 要求本文 |

### requestBody Properties
| Key | Value | Type | Description | Required | Format |
|:----------|:-------------|:-----|:------------|:------------|:------------|
| companyId | TW | String | 公司別代碼 | Y | n/a |
| depNumber | TW | Integer | 部門代碼 | Y | n/a |
| shiftYM | TW | String | 排班年月 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| visible | 是否顯示 |
| positionOption | 職稱 |
| gradeOption | 職級 |
| possieOption | 職位 |
| userTypeOption | 身分別 |
| placeOption | 工作地點 |
| employeesOption | 夥伴 |
| resultMessage | 結果訊息 |
| resultCode | 結果代號 |
| message | 訊息 |


### HTTP Response when Successful
```json
{
  "responseHeader": {
    "resultMessage": "執行成功",
    "resultCode": "200"
  },
  "responseBody": {
    "message": "查詢成功",
    "positionOption": {
      "id": "positionOption",
      "name": "職稱",
      "value": [
        {
          "code": "001",
          "name": "主管職(上級)",
          "ename": ""
        },
        {
          "code": "002",
          "name": "一般職(研究)",
          "ename": ""
        },
        {
          "code": "003",
          "name": "一般職(行政)",
          "ename": ""
        }
      ],
      "visible": true
    },
    "gradeOption": {
      "id": "gradeOption",
      "name": "職級",
      "value": [],
      "visible": false
    },
    "possieOption": {
      "id": "possieOption",
      "name": "職位",
      "value": [
        {
          "code": "0000",
          "name": "測試",
          "ename": ""
        },
        {
          "code": "0002",
          "name": "SA系統分析",
          "ename": ""
        }
      ],
      "visible": true
    },
    "userTypeOption": {
      "id": "userTypeOption",
      "name": "身分別",
      "value": [
        {
          "code": "A",
          "name": "正式人員",
          "ename": "formal Employee"
        },
        {
          "code": "B",
          "name": "特定性契約人員",
          "ename": ""
        }
      ],
      "visible": true
    },
    "placeOption": {
      "id": "placeOption",
      "name": "工作地點",
      "value": [
        {
          "code": "23",
          "name": "昆山",
          "ename": ""
        },
        {
          "code": "28",
          "name": "香港",
          "ename": ""
        }
      ],
      "visible": true
    },
    "employeesOption": {
        "id": "employeesOption",
        "name": "夥伴",
        "value": [
            {
                "code": "11203003",
                "name": "測OOOp t******p",
                "ename": ""
            },
            {
                "code": "admin",
                "name": "管O者 ",
                "ename": ""
            }
        ],
        "visible": true
    }
  }
}
```

### HTTP Response when No Data
無資料屬於正常情況
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"查無資料"
   }
}
```

### HTTP Response when Failed
```json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "500"
    },
    "responseBody": {
    }
}
```

### HTTP Response when Exception
```json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "406"
    },
    "responseBody": {
    }
}
```
