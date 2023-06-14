# apiExportExcel
匯出excel檔案

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiExportExcel
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
    "type":"xlsx"
    "companyId":"TW",
    "depNumber":495,
    "shiftYM":"202303",
    "startDate":"20230301",
    "endDate":"20230331",
    "allClass":[{
      "employeeId":"00001", 
      "employeeFullName":"王大帥"
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
| type | 類型(xls or xlsx) |
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
成功將直接顯示檔案blob，請務必參考content type
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
