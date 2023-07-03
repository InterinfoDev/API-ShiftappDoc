# apiRecognitionTerms
取得生物辨識條款

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiRecognitionTerms
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
      "locale":"TW"
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
| locale | TW | String | 條款語系 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| termsContent | 條款內容 |

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "termsContent": "判斷切換成英文語系，條款需要為英文語系的"
    }
}
```

### HTTP Response when No Data
{
    "responseHeader": {
        "resultMessage": "查無設定檔",
        "resultCode": "500"
    },
    "responseBody": {
        "termsContent": ""
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
