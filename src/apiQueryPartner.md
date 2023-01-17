# apiQueryPartner
查詢夥伴資訊

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryPartner
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
      "depNumber":,
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
| depNumber | "" | Integer | 部門代號 | n | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| empFullName | 中文姓名 |
| empFullEname | 英文姓名 |
| photo | 照片 |
| positionCode | 職稱代號 |
| phone | 手機號碼 |
| gradeCode | 職等代號 |
| possieCode | 職位代號 |
| positionName | 職稱名稱 |
| possieName | 職位名稱 |
| gradeName | 職等名稱 |
| userType | 身分別代號 |
| typeName | 身分別名稱 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"查詢成功",
      "employeeList":[
         {
            "empFullName":"晁O翔",
            "empFullEname":"NEW0896",
            "photo":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f28574d52634f57504b50637a726f605e5b52565111554f58",
            "positionCode":"5038",
            "phone":"0987XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"A",
            "typeName":"正式人員"
         },
         {
            "empFullName":"燕O雲",
            "empFullEname":"NEW0909",
            "photo":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f28574d52634f57504b50637a726f605e5b52565111554f58",
            "positionCode":"5058",
            "phone":"0987XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"A",
            "typeName":"正式人員"
         },
         {
            "empFullName":"文O瑾",
            "empFullEname":"NEW0937",
            "photo":"",
            "positionCode":"5058",
            "phone":"0912XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"A",
            "typeName":"正式人員"
         },
         {
            "empFullName":"蔚O鈞",
            "empFullEname":"NEW0991",
            "photo":"",
            "positionCode":"5048",
            "phone":"0912XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"A",
            "typeName":"正式人員"
         },
         {
            "empFullName":"瞿O裕",
            "empFullEname":"NEW1161",
            "photo":"",
            "positionCode":"5058",
            "phone":"0912XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"A",
            "typeName":"正式人員"
         },
         {
            "empFullName":"顧O棋",
            "empFullEname":"NEW1162",
            "photo":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f28574d52634f57504b50637a726f605e5b52565111554f58",
            "positionCode":"5048",
            "phone":"0987XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"A",
            "typeName":"正式人員"
         },
         {
            "empFullName":"仰O利",
            "empFullEname":"NEW1513",
            "photo":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f28574d52634f57504b50637a726f605e5b52565111554f58",
            "positionCode":"5003",
            "phone":"0987XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"短期契約",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"B",
            "typeName":"特定性契約人員"
         },
         {
            "empFullName":"宮O瑾",
            "empFullEname":"NEW1533",
            "photo":"",
            "positionCode":"5003",
            "phone":"0912XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"短期契約",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"B",
            "typeName":"特定性契約人員"
         },
         {
            "empFullName":"陳O明",
            "empFullEname":"NEWtest0009",
            "photo":"",
            "positionCode":"5001",
            "phone":"XXXXXXXXXXXXX",
            "gradeCode":"",
            "possieCode":"6715",
            "positionName":"系統管理員",
            "possieName":"海外行政高專",
            "gradeName":"",
            "userType":"A",
            "typeName":"正式人員"
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
