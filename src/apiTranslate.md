# apiTranslate
查詢裝置端翻譯資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiTranslate
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
| locale | TW | String | 語系 |
| deviceType | IOS | String | 裝置類型 |

### JSON representation
Here is a JSON representation of request.
```json
{
   "requestHeader":{
   },
   "requestBody":{
      "locale":"US",
      "deviceType":"IOS"
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
| locale | US | String | 語系 | Y | n/a |
| deviceType | IOS | String | 裝置類型 | Y | n/a 

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| messageId | 訊息代碼 |
| content | 翻譯內容 |
| resultMessage | 結果訊息 |
| resultCode | 結果代號 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "translateList":[
         {
            "content":"Name",
            "messageId":"employeeName"
         },
         {
            "content":"ID",
            "messageId":"empId"
         }
      ]
   }
}
```

### HTTP Response when No Data
無資料translateList回傳為空 
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "translateList":[]
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
