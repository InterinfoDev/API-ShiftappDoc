# apiQueryEmployee
取得人員資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryEmployee
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
      "employeeId":"0169"
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
| employeeId | 0169 | 查詢的員工編號 | Y | n/a |


### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| employeeId | 員工編號 |
| empFullName | 中文姓名 |
| empFullEname | 英文姓名 |
| photo | 照片 |
| depNumber | 部門代號(暗碼) |
| phone | 連絡電話 |
| address | 地址 |
| startDate | 開始日期 |
| placeCode | 工作地點代號 |
| depFullName | 部門全名 |
| depCode | 部門代號(明碼) |
| positionName | 職稱名稱 |
| placeName | 地點中文名稱 |
| placeEName | 工作地點英文名稱 |
| emergencyContactPhone | 緊急連絡電話 |
| emergencyContactName | 緊急連絡人姓名 |
| resultMessage | 結果訊息 |
| resultCode | 結果代號 |
| message | 訊息 |

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "message": "查詢成功",
        "employee": {
            "employeeId": "0169",
            "empFullName": "關Ｏ玲",
            "empFullEname": "NEW0169",
            "photo": "url",
            "depNumber": 1,
            "phone": "0987XXXXXXXXXXXXX",
            "address": "新北市中和區建八路16號",
            "startDate": "19891211",
            "placeCode": "TW3",
            "depFullName": "英特內股份有限公司",
            "depCode": "99999",
            "positionName": "",
            "possieName": "總處秘書",
            "placeName": "桃園",
            "placeEName": "",
            "emergencyContactPhone": "0932123456",
            "emergencyContactName": "林Ｏ明"
        },
        "chief": {
            "employeeId": "BBB01",
            "empFullName": "王Ｏ明",
            "empFullEname": ""
        }
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
