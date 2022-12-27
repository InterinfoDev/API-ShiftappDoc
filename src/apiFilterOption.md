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
| possieCode | 職稱代號 |
| possieName | 職稱名稱 |
| typeCode | 類型代碼 |
| typeName | 類型中文名稱 |
| typeEName | 類型英文名稱 |
| placeCode | 地點代碼 |
| placeName | 地點中文名稱 |
| placeEName | 地點英文名稱 |
| possieCode | 職稱代號 |
| possieName | 職稱名稱 |
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
      "gradeOption":[
         {
            "gradeCode":"1",
            "gradeName":"1"
         }
      ],
      "possieOption":[
         {
            "possieCode":"B-FT",
            "possieName":"外場-正職人員"
         },
         {
            "possieCode":"B-PT",
            "possieName":"外場-兼職人員"
         }
      ],
      "userTypeOption":[
         {
            "typeCode":"A",
            "typeName":"正職人員",
            "typeEName":""
         },
         {
            "typeCode":"B",
            "typeName":"建教生",
            "typeEName":""
         }
      ],
      "placeOption":[
         {
            "placeCode":"TW1",
            "placeName":"台北",
            "placeEName":""
         },
         {
            "placeCode":"TW10",
            "placeName":"嘉義",
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
