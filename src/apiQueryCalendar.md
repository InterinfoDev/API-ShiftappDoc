# apiQueryCalendar
取得行事曆日期和特別節日

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryCalendar
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
   "requestHeader":{
   },
   "requestBody":{
      "companyId":"TW",
      "calendarYM":"202303",
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
| companyId | TW | String | apiLogin所取得的companyId | Y | n/a |
| calendarYM | 202303 | String | 行事曆的年月 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| companyId | 公司別 |
| calendarYM | 行事曆年月 |
| date | 日期 |
| isHoliday | 是否為特定節日 |
| subject | 主題 |
| dayOfWeek | 星期 |
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
      "dateOutput":[
         {
            "date":"20230301",
            "dayOfWeek":3,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230302",
            "dayOfWeek":4,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230303",
            "dayOfWeek":5,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230304",
            "dayOfWeek":6,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230305",
            "dayOfWeek":0,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230306",
            "dayOfWeek":1,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230307",
            "dayOfWeek":2,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230308",
            "dayOfWeek":3,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230309",
            "dayOfWeek":4,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230310",
            "dayOfWeek":5,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230311",
            "dayOfWeek":6,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230312",
            "dayOfWeek":0,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230313",
            "dayOfWeek":1,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230314",
            "dayOfWeek":2,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230315",
            "dayOfWeek":3,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230316",
            "dayOfWeek":4,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230317",
            "dayOfWeek":5,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230318",
            "dayOfWeek":6,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230319",
            "dayOfWeek":0,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230320",
            "dayOfWeek":1,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230321",
            "dayOfWeek":2,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230322",
            "dayOfWeek":3,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230323",
            "dayOfWeek":4,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230324",
            "dayOfWeek":5,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230325",
            "dayOfWeek":6,
            "isHoliday":true,
            "subject":"清明-補班"
         },
         {
            "date":"20230326",
            "dayOfWeek":0,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230327",
            "dayOfWeek":1,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230328",
            "dayOfWeek":2,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230329",
            "dayOfWeek":3,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230330",
            "dayOfWeek":4,
            "isHoliday":false,
            "subject":""
         },
         {
            "date":"20230331",
            "dayOfWeek":5,
            "isHoliday":false,
            "subject":""
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
