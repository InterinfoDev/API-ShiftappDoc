# apiPinCode
驗證識別碼取得設定資訊

### HTTP Request
```
https://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiPinCode
```

### HTTP Request Mehod
```
POST
```

### JSON representation
Here is a JSON representation of request.
```json
{
   "requestHeader":{  
   },
   "requestBody":{
      "pinCode":"66666666"
   }
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
| pinCode | 97090920 | String | 授權碼 | Y | n/a |

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "result": true,
        "companyFullName": "英特內軟體",
        "file": "hrm8w.pkg",
        "domain": "http://www.interinfo.com.tw",
        "language": "TW",
        "message": "驗證成功"
    }
}
```

### HTTP Response when No Data
無資料屬於正常情況
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "result": false,
        "message": "授權碼錯誤 請重新輸入"
    }
}
```

### HTTP Response when Failed
```json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "5xx"
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
