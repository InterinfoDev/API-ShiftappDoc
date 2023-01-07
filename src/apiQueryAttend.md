# apiQueryAttend
夥伴查詢-考勤資訊

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
| attendDay | 出勤天數 |
| actualTotalHour | 實際出勤總時數 |
| scheduledTotalHour | 總預排出勤時數 |
| scheduledHour | 預排出勤時數 |
| actualHour | 實際出勤時數 |
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
      "attendDay":1.8,
      "actualTotalHour":18.0,
      "scheduledTotalHour":220.0,
      "attendanceList":[
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221205"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221206"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221207"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221208"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221209"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20221210"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20221211"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221212"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221213"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221214"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221215"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221216"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20221217"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20221218"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221219"
         },
         {
            "scheduledHour":10.0,
            "actualHour":10.0,
            "date":"20221220"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221221"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221222"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221223"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20221224"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20221225"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221226"
         },
         {
            "scheduledHour":10.0,
            "actualHour":8.0,
            "date":"20221227"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221228"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221229"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20221230"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20221231"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20230101"
         },
         {
            "scheduledHour":0.0,
            "actualHour":0.0,
            "date":"20230102"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20230103"
         },
         {
            "scheduledHour":10.0,
            "actualHour":0.0,
            "date":"20230104"
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
