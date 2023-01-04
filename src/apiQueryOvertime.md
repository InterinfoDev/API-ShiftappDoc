# apiQueryOvertime
查詢當月加班資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryOvertime
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

### Properties
| Property | Type | Description |
|:---------|:-----|:------------|
| requestHeader | Object | 要求本文 |
| requestBody | Object | 要求本文 |

### requestBody Properties
| Key | Value | Type | Description | Required | Format |
|:----------|:-------------|:-----|:------------|:------------|:------------|
| employeeId | admin | String | 員工編號 | Y | n/a |
| overtimeYM | 202201 | String | 查詢年月 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| resultMessage | 結果訊息 |
| resultCode | 結果代號 |
| message | 訊息 |
| totalHour | 當月總計時數 |
| hour | 加班時數 |
| date | 日期 |
| abnormal | 是否異常加班 |

### JSON representation
Here is a JSON representation of request.
```json
{
   "requestHeader":{
   },
   "requestBody":{
      "employeeId":"admin",
      "travelYM":"202201"
   },
   "uid":"98599308101484732326",
   "right":"51341911904173543336756162544864820"
}
```

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"查詢成功",
      "totalHour":8.0,
      "overtimeList":[
         {
            "hour":8.0,
            "date":"20220101",
            "abnormal":true
         },
         {
            "hour":0.0,
            "date":"20220102",
            "abnormal":false
         }
      ]
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
