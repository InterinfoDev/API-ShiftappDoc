# apiClassImport
排班Excel匯入

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiClassImport
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
      "depNumber": 495,
      "yymm": "202303",
      "file": ["202303排班表.xls","base64"],
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
| depNumber | 495 | Integer | 部門代號 | n | n/a |
| yymm | "202303" | String | 日期年月 | n | n/a |
| file | ["202303排班表.xls","base64"] | Array | 匯入檔案 | n | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| companyId | 公司別代碼 |
| depNumber | 部門代碼 |
| shiftYM | 排班日期年月 |
| startDate | 起始日期 |
| endDate | 結束日期 |
| classEmpolyeeList | 排班人員資料物件 |
| employeeId | 員工編號 |
| classImportExcelList | 排班資料物件 |
| classCode | 班別代碼 |
| vacationCode | 班轉假代碼 |
| date | 班轉假日期 |
| startTime | 起始時間 |
| endTime | 結束時間 |
| optionData | 全天，上半天，下半天 |
| specialDate | 特殊日期 |


### HTTP Response when Successful
```json
     {
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "companyId":"TW",
      "depNumber":495,
      "shiftYM":"202303",
      "startDate":"2023/03/01",
      "endDate":"2023/03/31",
      "classEmpolyeeList":[
         {
            "employeeId":"K20220035",
            "classImportExcelList":[
               {
                  "classCode":"00",
                  "vacationCode":"09",
                  "date":"20230301",
                  "startTime":"1500",
                  "endTime":"1800",
                  "optionData":"上半天",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"09",
                  "date":"20230302",
                  "startTime":"1500",
                  "endTime":"1800",
                  "optionData":"上半天",
                  "specialDate":"20230315"
               },
               {
                  "classCode":"00",
                  "vacationCode":"09",
                  "date":"20230303",
                  "startTime":"1500",
                  "endTime":"1800",
                  "optionData":"上半天",
                  "specialDate":"20230315"
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230304",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230305",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230306",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230307",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230308",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230309",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230310",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230311",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230312",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230313",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230314",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230315",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230316",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230317",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230318",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230319",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230320",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230321",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230322",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230323",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230324",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230325",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230326",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230327",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230328",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230329",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230330",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               },
               {
                  "classCode":"00",
                  "vacationCode":"",
                  "date":"20230331",
                  "startTime":"",
                  "endTime":"",
                  "optionData":"",
                  "specialDate":""
               }
            ]
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
