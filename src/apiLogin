# apiLogin
登入驗證並取得個人資訊

### HTTP Request
```
https://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiLogin
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

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "result":true,
      "message":"登入成功",
      "uid":"98599308101484732326",
      "right":"513419119041735433367561625448648202801232182995256636587932016607439201462466556235182663080673828674556200385271466125559349357786197118252096238747191633938599840684449342490964011524427764799493328110221539965006552590466959002677036856863519908176241437809573716163508936719855927717064013479997584572837246619648420374378288189675965452573416450376175273412420409191239097059629612395701880365980754522949348194952849418106023010387607494224029080312442356345333827742668253005042661612460080367422756341547727876278364154894157386843084143654173589798053183478405081380635",
      "companyId":"TW",
      "email":"admin@interinfo.com.tw",
      "empFullName":"系統管理員",
      "empFullEname":"Administrator",
      "photo":"Img base64",
      "depNumber":1,
      "depFullName":"英特內股份有限公司",
      "positionName":"系統管理員"
   }
}
```

### HTTP Response when No Data
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "result":false,
      "message":"帳號或密碼錯誤 請重新輸入"
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
