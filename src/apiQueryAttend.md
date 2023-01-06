# apiQueryAttend
夥伴列表-取得考勤資料

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryAttend
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
    "employeeId": "admin",
    "attendYM": "202212" 
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
| employeeId | admin | String | 員工編號 | Y | n/a |
| attendYM | 202212 | String | 年月 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| employeeId | 員工編號 |
| attendYM | 考勤年月 |
| attendYM | 出勤年月 |
| attendDays | 出勤天數 |
| attendTotalHours | 實際出勤總時數 |
| attendTotalScheduledHours | 總預排出勤時數 |
| scheduledAttendHours | 預排出勤時數 |
| actualAttendHours | 實際出勤時數 |
| date |日期 |
| week | 星期 |
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
      "attendYM":"202212",
      "attendDays":"31",
      "attendTotalHours":"18",
      "attendTotalScheduledHours":"220",
      "attendanceList":[
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221205",
            "week":"(一)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221206",
            "week":"(二)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221207",
            "week":"(三)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221208",
            "week":"(四)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221209",
            "week":"(五)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20221210",
            "week":"(六)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20221211",
            "week":"(日)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221212",
            "week":"(一)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221213",
            "week":"(二)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221214",
            "week":"(三)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221215",
            "week":"(四)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221216",
            "week":"(五)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20221217",
            "week":"(六)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20221218",
            "week":"(日)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221219",
            "week":"(一)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"10.0",
            "date":"20221220",
            "week":"(二)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221221",
            "week":"(三)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221222",
            "week":"(四)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221223",
            "week":"(五)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20221224",
            "week":"(六)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20221225",
            "week":"(日)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221226",
            "week":"(一)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"8.0",
            "date":"20221227",
            "week":"(二)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221228",
            "week":"(三)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221229",
            "week":"(四)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20221230",
            "week":"(五)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20221231",
            "week":"(六)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20230101",
            "week":"(日)"
         },
         {
            "scheduledAttend":"0.0",
            "actualAttend":"0.0",
            "date":"20230102",
            "week":"(一)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20230103",
            "week":"(二)"
         },
         {
            "scheduledAttend":"10.0",
            "actualAttend":"0.0",
            "date":"20230104",
            "week":"(三)"
         }
      ]
   }
}
```

### HTTP Response when No Data

此程式不會有查無資料發生

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
