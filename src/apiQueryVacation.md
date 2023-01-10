# apiQueryVacation
查詢請假頁資料

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryVacation
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
| employeeId | 0169 | String | 員工編號 | Y | n/a |
| vacationYM | 202203 | String | 年月 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| resultMessage | 結果訊息 |
| resultCode | 結果代號 |
| message | 訊息 |
| vacationName | 假別 |
| startDate | 開始日期 |
| startTime | 開始時間 |
| endDate | 結束日期 |
| endTime | 結束時間 |
| amt | 時數/天數 |
| reason | 請假原因 |
| agent | 代理人 |
| colorCode | 假別色碼 |


### JSON representation
Here is a JSON representation of request.
```json
{
   "requestHeader":{
   },
   "requestBody":{
      "employeeId":"0169",
      "vacationYM":"202203"
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
      "annualLeave":{
         "totalAmt":70.0,
         "usedAmt":0.0,
         "unit":"天"
      },
      "vacationList":[
         {
            "vacationName":"休息",
            "startDate":"01/23(一)",
            "endDate":"01/23(一)",
            "startTime":"09:00",
            "endTime":"18:00",
            "unit": "小時",
            "reason":"test",
            "agent":"2O3",
            "colorCode":"6B6B75",
            "amt": 8.0
         }
      ]
   }
}
```

### HTTP Response when No Data
```json
{
  "responseHeader": {
    "resultMessage": "執行成功",
    "resultCode": "200"
  },
  "responseBody": {
    "message": "查無資料",
    "travelList": []
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
