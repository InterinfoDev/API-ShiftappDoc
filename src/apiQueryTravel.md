# apiQueryTravel
查詢出差

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryTravel
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

### Properties
| Property | Type | Description |
|:---------|:-----|:------------|
| requestHeader | Object | 要求本文 |
| requestBody | Object | 要求本文 |

### requestBody Properties
| Key | Value | Type | Description | Required | Format |
|:----------|:-------------|:-----|:------------|:------------|:------------|
| employeeId | 0169 | String | 員工編號 | Y | n/a |
| travelYM | 202203 | String | 年月 | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| resultMessage | 結果訊息 |
| resultCode | 結果代號 |
| message | 訊息 |
| startDate | 開始日期 |
| startTime | 開始時間 |
| endDate | 結束日期 |
| endTime | 結束時間 |
| place | 	工作地點名稱 |
| workingItem | 辦理事項 |
| note | 備註/說明 |

### JSON representation
Here is a JSON representation of request.
```json
{
   "requestHeader":{
   },
   "requestBody":{
      "employeeId":"0169",
      "travelYM":"202203"
   },
   "uid":"98599308101484732326",
   "right":"51341911904173543336756162544864820"
}
```

### HTTP Response when Successful
```json
{
  "responseHeader": {
    "resultMessage": "執行成功",
    "resultCode": "200"
  },
  "responseBody": {
    "message": "查詢成功",
    "travelList": [
      {
        "startDate": "20220312",
        "endDate": "20220312",
        "startTime": "0800",
        "endTime": "1700",
        "place": "南港中國信託",
        "workingItem": "外訓",
        "note": "餐費100 + 車票50"
      },
      {
        "startDate": "20220304",
        "endDate": "20220307",
        "startTime": "0800",
        "endTime": "1700",
        "place": "台北南港",
        "workingItem": "外訓",
        "note": "AndyHou測試出差單備註"
      }
    ]
  }
}
```

### HTTP Response when No Data
```json
{
  "responseHeader": {
    "resultMessage": "執行成功",
    "resultCode": "200"
  },
  "responseBody": {
    "message": "查無資料",
    "travelList": []
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
