# apiHomePage
排班首頁-預設值

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiHomePage
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
    "shiftYM":"202303",
    "depNumber":495
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
| employeeId | 員工編號 |
| empFullName | 中文姓名 |
| empFullEname | 英文姓名 |
| sex | 性別 |
| depNumber | 部門暗碼 |
| depFullName | 部門名稱 |
| depCode | 部門代號 |
| positionCode | 職稱代碼 |
| positionName | 職稱名稱 |
| placeCode | 工作地點代碼 |
| placeName | 工作地點名稱 |
| placeEName | 工作地點英文名稱 |
| gradeCode | 職級代碼 |
| gradeName | 職級名稱 |
| possieCode | 職位代碼 |
| possieName | 職位名稱 |
| userType | 身分別代碼 |
| typeName | 身分別名稱 |
| typeEName | 身分別英文名稱 |
| support | 是否為支援人力 |
| saveKey | 存取資料Key |
| date | 排班日期 |
| classCode | 班別代號 |
| className | 班別名稱 |
| classCo | 班別代號 |
| classCode | 班別代號 |
| startTime | 班別起始時間 |
| endTime | 班別結束時間 |
| workHour | 班別工時 |
| edit | 是否可編輯 |
| startDate | 考勤起日 |
| endDate | 考勤迄日 |
| totalHour | 部門排班時數上限 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "attend":{
         "startDate":"20230301",
         "endDate":"20230331",
         "totalHour":0.0
      },
      "employeeList":[
         {
            "employeeId": "0019",
            "empFullName": "習O庭",
            "empFullEname": "NEW0019",
            "depNumber": 495,
            "depFullName": "企劃部",
            "depCode": "55",
            "sex": "M",
            "photo": "",
            "positionCode": "5076",
            "placeCode": "TW2",
            "gradeCode": "11",
            "gradeName": "11",
            "possieCode": "6715",
            "positionName": "正工程師(一)",
            "possieName": "海外行政高專",
            "placeName": "新北",
            "placeEName": "",
            "userType": "A",
            "typeName": "正式人員",
            "typeEName": "formal Employee",
            "support": false,
            "saveKey": "108228376095740581741",
            "shiftList":[
               {
                  "date":"20230301",
                  "classInfo": {
                      "classCode": "04",
                      "className": "夜班",
                      "startTime": "1600",
                      "endTime": "2130",
                      "workHour": 8.0
                  },
                  "edit": true
               },
               {
                  "date":"20230302",
                  "classInfo": {
                      "classCode": "04",
                      "className": "夜班",
                      "startTime": "1600",
                      "endTime": "2130",
                      "workHour": 8.0
                  },
                  "edit": true
               },
               {
                  "date":"20230303",
                  "classInfo": {
                      "classCode": "O",
                      "className": "例假日",
                      "startTime": "",
                      "endTime": "",
                      "workHour": 0.0
                  },
                  "edit": true
               }
            ]
         }
      ],
      "message":"查詢成功"
   }
}
```

### HTTP Response when No Data
{
  "responseHeader": {
    "resultMessage": "執行成功",
    "resultCode": "200"
  },
  "responseBody": {
    "attend": {
      "startDate": "20230301",
      "endDate": "20230331",
      "totalHour": 0.0
    },
    "employeeList": [],
    "message": "查詢成功"
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
