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
          "positionCode": "001",
          "positionName": "主管職(上級)"
        },
        {
          "positionCode": "002",
          "positionName": "一般職(研究)"
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
          "possieCode": "0000",
          "possieName": "測試"
        },
        {
          "possieCode": "0002",
          "possieName": "SA系統分析"
        }
      ],
      "visible": true
    },
    "userTypeOption": {
      "id": "userTypeOption",
      "name": "身分別",
      "value": [
        {
          "typeCode": "A",
          "typeName": "正式人員",
          "typeEName": "formal Employee"
        },
        {
          "typeCode": "B",
          "typeName": "特定性契約人員",
          "typeEName": ""
        },
        {
          "typeCode": "C",
          "typeName": "外籍人士",
          "typeEName": ""
        },
        {
          "typeCode": "D",
          "typeName": "台灣幹部",
          "typeEName": ""
        },
        {
          "typeCode": "E",
          "typeName": "一般契約人員",
          "typeEName": ""
        },
        {
          "typeCode": "F",
          "typeName": "外派人員",
          "typeEName": ""
        }
      ],
      "visible": true
    },
    "placeOption": {
      "id": "placeOption",
      "name": "工作地點",
      "value": [
        {
          "placeCode": "23",
          "placeName": "昆山",
          "placeEName": ""
        },
        {
          "placeCode": "28",
          "placeName": "香港",
          "placeEName": ""
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
