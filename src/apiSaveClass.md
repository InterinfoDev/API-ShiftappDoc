# apiSaveClass
排班送出

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiSaveClass
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
    "companyId":"TW",
    "depNumber":495,
    "shiftYM":"202304",
    "startDate":"20230401",
    "endDate":"20230408",
    "allClass":[{
      "employeeId":"00001", 
       "dailyClass":[{
        "classCode":"00", 
        "vacationCode":"", 
        "date":"20230401", 
        "startTime":"", 
        "endTime":"", 
        "optionData":"", 
        "specialDate":""
        }]
       }]
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

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| companyId | 公司別 |
| depNumber | 部門代碼 |
| shiftYM | 排班年月 |
| startDate | 排班起始日期 |
| endDate | 排班結束日期 |
| employeeId | 員工編號 |
| classCode | 畫面上填寫的班別代碼 |
| vacationCode | 班轉假代碼 |
| date | 排班日期 |
| startTime | 班轉假起始時間 |
| endTime | 班轉假結束時間 |
| optionData | 班轉假請假時段 |
| specialDate | 班轉假特殊日期 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"檢核完成，點選夥伴姓名，查看檢核結果",
      "verify":false,
      "result":[
         {
            "check":[
               "員工編號：00001(報表一TEST1105)，2023/04月休應為10.0天，目前排休11.0天，是否繼續"
            ],
            "error":[
               "員工編號：00001(報表一TEST1105)，從20230327連續排上班至20230402總計7天已超過7天"
            ],
            "employeeId":"00001"
         }
      ]
   }
}
```

### HTTP Response when No Data
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"送出成功",
      "success":true,
      "result":[]
   }
}


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
