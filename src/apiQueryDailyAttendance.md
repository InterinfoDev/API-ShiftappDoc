# apiQueryDailyAttendance
查詢本日出勤表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryDailyAttendance
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
      "depNumber": 495,
      "date": "20230314",
      "companyId":"TW",
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
| depNumber | 495 | Integer | 部門代碼 | n | n/a |
| date | "20230315" | String | 日期 | n | n/a |
| companyId | "TW" | String | 公司別 | n | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| keyName | 中文名稱 |
| keyEngName | 英文名稱 |
| keyPeople | 人數 |
| attendanceDetailList | 員工資料 |
| photo | 照片 |
| empFullName | 中文姓名 |
| empFullEngName | 英文姓名 |
| workClass | 班別代碼 |
| classStartTime | 班別起始時間 |
| classEndTime | 班別結束時間 |
| inCard | 進卡時間 |
| outCard | 出卡時間 |
| attendState | 考勤狀態 |
| state | 狀態 |
| textColor | 字色色碼 |
| baseColor | 底色色碼 |
| errorSort | 異常排序規則|

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "message": "查詢成功",
        "attendanceList": [
            {
                "key": "allPeople",
                "title": "單位總人數",
                "visible": true,
                "people": 3,
                "attendanceDetailList": [
                    {
                        "photo": "hrm/photo/1697528779798_200109_AdoptingKoala08.jpg",
                        "employeeId": "10108001",
                        "empFullName": "鄭O隆",
                        "empFullEngName": "L***y",
                        "workClass": "D",
                        "workClassName": "總公司班",
                        "classStartTime": "0900",
                        "classEndTime": "1800",
                        "inCard": "",
                        "outCard": "",
                        "attendState": [
                            {
                                "tag": "曠職",
                                "textColor": "B53CFF",
                                "baseColor": "F0D8FF"
                            }
                        ],
                        "errorSort": 6
                    },
                    {
                        "photo": "hrm/photo/1677145343441_貓LOG測試.jpg",
                        "employeeId": "10905012",
                        "empFullName": "蔣O菱",
                        "empFullEngName": "V**a",
                        "workClass": "D",
                        "workClassName": "總公司班",
                        "classStartTime": "0900",
                        "classEndTime": "1800",
                        "inCard": "",
                        "outCard": "",
                        "attendState": [],
                        "errorSort": 1
                    },
                    {
                        "photo": "hrm/photo/1677145343441_貓LOG測試.jpg",
                        "employeeId": "11001024",
                        "empFullName": "白O閔",
                        "empFullEngName": "J****n",
                        "workClass": "D",
                        "workClassName": "總公司班",
                        "classStartTime": "0900",
                        "classEndTime": "1800",
                        "inCard": "",
                        "outCard": "",
                        "attendState": [
                            {
                                "tag": "曠職",
                                "textColor": "B53CFF",
                                "baseColor": "F0D8FF"
                            }
                        ],
                        "errorSort": 6
                    }
                ]
            },
            {
                "key": "exemptAttend",
                "title": "免出勤",
                "visible": true,
                "people": 0,
                "attendanceDetailList": []
            },
            {
                "key": "shouldAttend",
                "title": "應出勤",
                "visible": true,
                "people": 2,
                "attendanceDetailList": [
                    {
                        "photo": "hrm/photo/1697528779798_200109_AdoptingKoala08.jpg",
                        "employeeId": "10108001",
                        "empFullName": "鄭O隆",
                        "empFullEngName": "L***y",
                        "workClass": "D",
                        "workClassName": "總公司班",
                        "classStartTime": "0900",
                        "classEndTime": "1800",
                        "inCard": "",
                        "outCard": "",
                        "attendState": [
                            {
                                "tag": "曠職",
                                "textColor": "B53CFF",
                                "baseColor": "F0D8FF"
                            }
                        ],
                        "errorSort": 6
                    },
                    {
                        "photo": "hrm/photo/1677145343441_貓LOG測試.jpg",
                        "employeeId": "11001024",
                        "empFullName": "白O閔",
                        "empFullEngName": "J****n",
                        "workClass": "D",
                        "workClassName": "總公司班",
                        "classStartTime": "0900",
                        "classEndTime": "1800",
                        "inCard": "",
                        "outCard": "",
                        "attendState": [
                            {
                                "tag": "曠職",
                                "textColor": "B53CFF",
                                "baseColor": "F0D8FF"
                            }
                        ],
                        "errorSort": 6
                    }
                ]
            },
            {
                "key": "vacation",
                "title": "請假",
                "visible": true,
                "people": 0,
                "attendanceDetailList": []
            },
            {
                "key": "travel",
                "title": "出差",
                "visible": true,
                "people": 1,
                "attendanceDetailList": [
                    {
                        "photo": "hrm/photo/1677145343441_貓LOG測試.jpg",
                        "employeeId": "10905012",
                        "empFullName": "蔣O菱",
                        "empFullEngName": "V**a",
                        "workClass": "D",
                        "workClassName": "總公司班",
                        "classStartTime": "0900",
                        "classEndTime": "1800",
                        "inCard": "",
                        "outCard": "",
                        "attendState": [],
                        "errorSort": 1
                    }
                ]
            },
            {
                "key": "notCard",
                "title": "應刷未刷",
                "visible": false,
                "people": 0,
                "attendanceDetailList": []
            },
            {
                "key": "absent",
                "title": "曠職",
                "visible": true,
                "people": 2,
                "attendanceDetailList": [
                    {
                        "photo": "hrm/photo/1697528779798_200109_AdoptingKoala08.jpg",
                        "employeeId": "10108001",
                        "empFullName": "鄭O隆",
                        "empFullEngName": "L***y",
                        "workClass": "D",
                        "workClassName": "總公司班",
                        "classStartTime": "0900",
                        "classEndTime": "1800",
                        "inCard": "",
                        "outCard": "",
                        "attendState": [
                            {
                                "tag": "曠職",
                                "textColor": "B53CFF",
                                "baseColor": "F0D8FF"
                            }
                        ],
                        "errorSort": 6
                    },
                    {
                        "photo": "hrm/photo/1677145343441_貓LOG測試.jpg",
                        "employeeId": "11001024",
                        "empFullName": "白O閔",
                        "empFullEngName": "J****n",
                        "workClass": "D",
                        "workClassName": "總公司班",
                        "classStartTime": "0900",
                        "classEndTime": "1800",
                        "inCard": "",
                        "outCard": "",
                        "attendState": [
                            {
                                "tag": "曠職",
                                "textColor": "B53CFF",
                                "baseColor": "F0D8FF"
                            }
                        ],
                        "errorSort": 6
                    }
                ]
            },
            {
                "key": "attend",
                "title": "實際出勤",
                "visible": true,
                "people": 0,
                "attendanceDetailList": []
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
