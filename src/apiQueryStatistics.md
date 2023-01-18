# apiQueryStatistics
取得統計報表

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryStatistics
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
      "companyId":"TW",
      "depNumber":528,
      "shiftYM":"202212"
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
| companyId | TW | String | apiLogin所取得的companyId | Y | n/a |
| depNumber | 534 | Integer | 部門 | N | n/a |
| attendYM | 202212 | String | 考勤年月 | N | YYYYmm |
| positionCode |  | String | 職稱 | N | n/a |
| userType |  | String | 身分別 | N | n/a |
| possieCode |  | String | 職位 | N | n/a |


### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| attendYM | 考勤年月 |
| date | 日期 |
| resultMessage | 結果訊息 |
| resultCode | 結果代號 |
| message | 訊息 |
| actualAttendTotalHours | 實際出勤總計時數 |
| scheduledAttendTotalHours | 預排出勤總計時數 |
| supportTotalHours | 支援借調總計時數 |
| monthTotalHours | 出勤合計總計時數 |
| holidayTotalHours | 休假/免出勤總計時數 |
| actualAttendTotalPeople | 實際出勤總計人數 |
| scheduledAttendTotalPeople | 預排出勤總計人數 |
| supportTotalPeople | 支援借調總計人數 |
| monthTotalPeople | 出勤合計總計人數 |
| holidayTotalPeople | 休假/免出勤總計人數 |
| overtimeTotalHours | 加班時數總計 |
| overtimeTotalPeople | 加班人數總計 |
| attendHoursStatisticsList | 出勤時數列表 |
| scheduledHours | 每日預排出勤時數 |
| actualHours | 每日實際出勤時數 |
| supportHours | 每日支援借調時數 |
| dayTotalHours | 每日出勤合計時數 |
| holidayHours | 每日休假 / 免出勤時數 |
| attendPeopleStatisticsList | 出勤人數列表 |
| scheduledPeople | 每日預排出勤人數 |
| actualPeople | 每日實際出勤人數 |
| supportPeople | 每日支援借調人數 |
| dayTotalPeople | 每日出勤合計人數 |
| overtimeStatisticsList | 加班統計列表 |
| overtimePeople | 每日加班人數 |
| overtimeHours | 每日加班時數 |

### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "message": "查詢成功",
        "attendYM": "202112",
        "actualAttendTotalHours": 0.0,
        "scheduledAttendTotalHours": 2093.0,
        "supportTotalHours": 0.0,
        "monthTotalHours": 0.0,
        "holidayTotalHours": 0.0,
        "actualAttendTotalPeople": 0,
        "scheduledAttendTotalPeople": 253,
        "supportTotalPeople": 0,
        "monthTotalPeople": 0,
        "holidayTotalPeople": 0,
        "overtimeTotalHours": 0.0,
        "overtimeTotalPeople": 0,
        "attendHoursStatisticsList": [
            {
                "scheduledHours": 91.0,
                "actualHours": 0.0,
                "supportHours": 0.0,
                "dayTotalHours": 0.0,
                "holidayHours": 0.0,
                "date": "20211201"
            },
            {
                "scheduledHours": 91.0,
                "actualHours": 0.0,
                "supportHours": 0.0,
                "dayTotalHours": 0.0,
                "holidayHours": 0.0,
                "date": "20211202"
            }
        ],
        "attendPeopleStatisticsList": [
            {
                "scheduledPeople": 11,
                "actualPeople": 0,
                "supportPeople": 0,
                "dayTotalPeople": 0,
                "holidayPeople": 0,
                "date": "20211201"
            },
            {
                "scheduledPeople": 11,
                "actualPeople": 0,
                "supportPeople": 0,
                "dayTotalPeople": 0,
                "holidayPeople": 0,
                "date": "20211202"
            },

        ],
        "overtimeStatisticsList": [
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211201"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211202"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211203"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211204"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211205"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211206"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211207"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211208"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211209"
            },
            {
                "overtimePeople": 0,
                "overtimeHours": 0.0,
                "date": "20211210"
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
