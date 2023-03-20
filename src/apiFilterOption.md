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
    "companyId": "TW"
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

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| gradeCode | 職等代號 |
| gradeName | 職等名稱 |
| PositionCode | 職稱代號 |
| PositionName | 職稱名稱 |
| typeCode | 類型代碼 |
| typeName | 類型中文名稱 |
| typeEName | 類型英文名稱 |
| placeCode | 地點代碼 |
| placeName | 地點中文名稱 |
| placeEName | 地點英文名稱 |
| possieCode | 職位代號 |
| possieName | 職位名稱 |
| resultMessage | 結果訊息 |
| resultCode | 結果代號 |
| message | 訊息 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"查詢成功",
      "positionOption":[
         {
            "positionCode":"ha123",
            "positionName":"哈哈約聘人員"
         },
         {
            "positionCode":"P01",
            "positionName":"職稱1"
         },
         {
            "positionCode":"P02",
            "positionName":"職稱2"
         },
         {
            "positionCode":"P03",
            "positionName":"基層幹部1"
         },
         {
            "positionCode":"S001",
            "positionName":"行政人員"
         },
         {
            "positionCode":"S002",
            "positionName":"HR主管"
         },
         {
            "positionCode":"S003",
            "positionName":"顧問工程師"
         },
         {
            "positionCode":"S004",
            "positionName":"外籍勞工"
         }
      ],
      "gradeOption":[
         {
            "gradeCode":"06",
            "gradeName":"06"
         }
      ],
      "possieOption":[
         {
            "possieCode":"3712",
            "possieName":"技術服務專員"
         },
         {
            "possieCode":"3941",
            "possieName":"運輸業務高專"
         },
         {
            "possieCode":"4112",
            "possieName":"製程操作員"
         },
         {
            "possieCode":"4113",
            "possieName":"製程技術專員"
         },
         {
            "possieCode":"4122",
            "possieName":"包裝操作員"
         },
         {
            "possieCode":"4151",
            "possieName":"粉體押出員"
         }
      ],
      "userTypeOption":[
         {
            "typeCode":"C",
            "typeName":"外籍人士",
            "typeEName":""
         },
         {
            "typeCode":"D",
            "typeName":"台灣幹部",
            "typeEName":""
         },
         {
            "typeCode":"E",
            "typeName":"一般契約人員",
            "typeEName":""
         },
         {
            "typeCode":"F",
            "typeName":"外派人員",
            "typeEName":""
         }
      ],
      "placeOption":[
         
         {
            "placeCode":"TW5",
            "placeName":"苗栗",
            "placeEName":""
         },
         {
            "placeCode":"TW6",
            "placeName":"台中",
            "placeEName":""
         },
         {
            "placeCode":"TW7",
            "placeName":"彰化",
            "placeEName":""
         },
         {
            "placeCode":"TW8",
            "placeName":"南投",
            "placeEName":""
         },
         {
            "placeCode":"TW9",
            "placeName":"雲林",
            "placeEName":""
         },
         {
            "placeCode":"V01",
            "placeName":"綿陽市",
            "placeEName":""
         },
         {
            "placeCode":"V02",
            "placeName":"廣元市",
            "placeEName":""
         },
         {
            "placeCode":"V03",
            "placeName":"南充市",
            "placeEName":""
         },
         {
            "placeCode":"V04",
            "placeName":"巴中市",
            "placeEName":""
         },
         {
            "placeCode":"V05",
            "placeName":"達州市",
            "placeEName":""
         }
      ]
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
