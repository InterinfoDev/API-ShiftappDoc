# apiWorkClassOption
取得班別資料

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiWorkClassOption
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
    "depNumber": 1 ,
    "favorite": null
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

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| classCode | 班別代碼 |
| workHour | 工作時數 |
| startTime | 開始時間 |
| favorite | 常用 |
| endTime | 結束時間 |
| isClassToVaca | 是否為班轉假 |
| vacationCode | 班轉假的假別代碼 |
| vacationName | 班轉假假別名稱 |
| vacationEdit | 特殊日期欄位可不可以編輯 |
| vacationOption | 下拉選項，如果是班轉假且此欄位為空，那輸入方式為時間輸入(也就是有兩個輸入框) |
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
      "workClassOption":[
         {
            "classCode":"01",
            "className":"通用班(8-17)",
            "startTime":"0830",
            "endTime":"1730",
            "workHour":8.0,
            "favorite":true,
            "isClassToVaca": true, 
            "vacationCode": "M70",
            "vacationName": "婚假(天)",
            "vacationEdit": true,
            "vacationOption": [
                {
                    "optionName": "請全天",
                    "optionData": "all"
                }
            ]
         },
         {
            "classCode":"02-1",
            "className":"(08-12)",
            "startTime":"0800",
            "endTime":"1200",
            "workHour":4.0,
            "favorite":false,
            "isClassToVaca": true, 
            "vacationCode": "M70",
            "vacationName": "婚假(天)",
            "vacationEdit": true,
            "vacationOption": [
                {
                    "optionName": "請全天",
                    "optionData": "all"
                }
            ]
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
      "message":"查無資料",
      "workClassOption":[]
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
