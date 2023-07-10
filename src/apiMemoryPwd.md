# apiMemoryPwd
生物辨識記憶密碼驗證員工登入密碼

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiMemoryPwd
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
      "uid":"admin",
      "pwd":"admin"
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
| uid | admin | String | 使用者帳號 | Y | n/a |
| pwd | admin | String | 使用者密碼 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| result | 驗證結果 |
| message | 驗證訊息 |

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "result": true
    }
}
```

### HTTP Response when Failed
```json
{
    "responseHeader": {
        "resultMessage": "驗證失敗，請重新確認帳號密碼",
        "resultCode": "500"
    },
    "responseBody": {
        "result": false
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
