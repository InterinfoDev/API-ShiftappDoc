# apiLogin
登入驗證並取得個人資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiLogin
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
| companyId | 公司別 |
| email | 信箱帳號 |
| empFullName | 中文姓名 |
| empFullEname | 英文姓名 |
| sex | 性別 |
| photo | 照片 |
| depNumber | 部門代號(暗碼) |
| depFullName | 部門全名 |
| positionName | 職稱名稱 |
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
      "message":"登入成功",
      "uid":"98599308101484732326",
      "right":"513419119041735433367561625448648202801232182995256636587932016607439201462466556235182663080673828674556200385271466125559349357786197118252096238747191633938599840684449342490964011524427764799493328110221539965006552590466959002677036856863519908176241437809573716163508936719855927717064013479997584572837246619648420374378288189675965452573416450376175273412420409191239097059629612395701880365980754522949348194952849418106023010387607494224029080312442356345333827742668253005042661612460080367422756341547727876278364154894157386843084143654173589798053183478405081380635",
      "companyId":"TW",
      "email":"admin@interinfo.com.tw",
      "empFullName":"系統管理員",
      "empFullEname":"Administrator",
      "photo":"Img base64",
      "sex":"F",
      "depNumber":1,
      "depFullName":"英特內股份有限公司",
      "positionName":"系統管理員"
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
