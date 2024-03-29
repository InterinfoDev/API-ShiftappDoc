# apiQueryDaily
取得每日資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryDaily
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
      "depNumber":528,
      "startDate":"20231113",
      "endDate":"20231113"
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
| depNumber | 528 | Integer | apiFilterOption所選的部門 | Y | n/a |
| startDate | 20221201 | String | 起始日期 | Y | YYYYmmdd |
| endDate | 20221201 | String | 結束日期 | Y | YYYYmmdd |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| startDate | 考勤起始日期 |
| endDate | 考勤結束日期 |
| date | 日期 |
| note | 備註/說明 |
| supportCount | 支援數量 |
| vacationCount | 休假天數 |
| employeeId | 員工編號 |
| empFullName | 中文姓名 |
| depFullName | 部門全名 |
| isHoliday | 是否為國定假日 |
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
      "message":"查詢成功",
      "attend":{
         "startDate":"20221201",
         "endDate":"20221231"
      },
      "dailyInfo":[
         {
            "date":"20221201",
            "subject":"二二八紀念日",
            "dayOfWeek":"週二",
            "isHoliday":true,
            "note":"kevin假資料測試",
            "supportCount":3,
            "vacationCount":1,
            "supportDetail":[
               {
                  "employeeId":"0060",
                  "empFullName":"歐O庭",
                  "depFullName":"顧問處"
               },
               {
                  "employeeId":"0310",
                  "empFullName":"卓O伶",
                  "depFullName":"顧問處"
               },
               {
                  "employeeId":"1090",
                  "empFullName":"蔡O凌",
                  "depFullName":"顧問處"
               }
            ]
         },
         {
            "date":"20221202",
            "subject":"週一．二二八紀念日",
            "dayOfWeek":"週二",
            "isHoliday":true,
            "note":"kevin假資料測試",
            "supportCount":3,
            "vacationCount":1,
            "supportDetail":[
               {
                  "employeeId":"0060",
                  "empFullName":"歐O庭",
                  "depFullName":"顧問處"
               },
               {
                  "employeeId":"0310",
                  "empFullName":"卓O伶",
                  "depFullName":"顧問處"
               },
               {
                  "employeeId":"1090",
                  "empFullName":"蔡O凌",
                  "depFullName":"顧問處"
               }
            ]
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
