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
| phone | 連絡電話 |
| address | 地址 |
| startDate | 開始日期 |
| placeName | 工作地點 |
| depFullName | 工作單位 |
| positionName | 職稱名稱 |
| gradeName | 職等 |
| possieName | 職位 |
| userTypeName | 身份別 |
| placeName | 地點中文名稱 |
| directChief | 直屬主管 |
| agentName | 職務代理人 |
| phone | 行動電話 |
| mail | 電子信箱 |
| emergencyContactPhone | 緊急連絡電話 |
| emergencyContactName | 緊急連絡人姓名 |
| emergencyContactRelationship | 緊急連絡人關係 |
| disease | 歷史疾病 |
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
         "employeeFileDetail":[
         {
            "id":"photo",
            "name":"照片",
            "value":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "visable":true
         },
         {
            "id":"employeeId",
            "name":"員工編號",
            "value":"admin",
            "visable":true
         },
         {
            "id":"empFullName",
            "name":"中文姓名",
            "value":"系統管理員",
            "visable":true
         },
         {
            "id":"empFullEname",
            "name":"英文姓名",
            "value":"eline",
            "visable":true
         },
         {
            "id":"depFullName",
            "name":"工作單位",
            "value":"企劃部",
            "visable":true
         },
         {
            "id":"placeName",
            "name":"工作地點",
            "value":"雲林",
            "visable":true
         },
         {
            "id":"startDate",
            "name":"到職日",
            "value":"",
            "visable":false
         },
         {
            "id":"directChief",
            "name":"直屬主管",
            "value":"池O祥",
            "visable":true
         },
         {
            "id":"positionName",
            "name":"職稱",
            "value":"系統管理員",
            "visable":true
         },
         {
            "id":"gradeName",
            "name":"職等",
            "value":"",
            "visable":true
         },
         {
            "id":"possieName",
            "name":"職位",
            "value":"SA系統分析",
            "visable":true
         },
         {
            "id":"userTypeName",
            "name":"身份別",
            "value":"",
            "visable":false
         },
         {
            "id":"agentName",
            "name":"職務代理人",
            "value":"",
            "visable":true
         },
         {
            "id":"phone",
            "name":"行動電話",
            "value":"",
            "visable":false
         },
         {
            "id":"mail",
            "name":"電子信箱",
            "value":"",
            "visable":false
         },
         {
            "id":"emergencyContactName",
            "name":"緊急聯絡人姓名",
            "value":"測試B",
            "visable":true
         },
         {
            "id":"emergencyContactRelationship",
            "name":"緊急連絡人關係",
            "value":"",
            "visable":false
         },
         {
            "id":"emergencyContactPhone",
            "name":"緊急連絡人行動電話",
            "value":"0932-123456",
            "visable":true
         },
         {
            "id":"disease",
            "name":"員工身體狀況",
            "value":"",
            "visable":true
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
