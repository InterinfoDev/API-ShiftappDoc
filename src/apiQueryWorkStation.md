# apiQueryWorkStation
查詢工作站

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryWorkStation
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
      "depNumber": 24,
      "date": "20230410",
      "companyId":"1"
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

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| time | 時段 |
| stationInfo | 工作站資訊 |
| branchPeopleCount | 工作子站人數 |
| branchStationName | 工作子站名稱 |
| branchStationCode | 工作子站代號 |
| peopleInfo | 員工資料 |
| employeePhoto | 照片 |
| empFullName | 中文姓名 |
| empFullEngName | 英文姓名 |
| employeeId | 員工編號 |

### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"查詢成功",
      "timeBlock":[
         {
            "time":"0800",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               }
            ]
         },
         {
            "time":"0830",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               }
            ]
         },
         {
            "time":"0900",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               }
            ]
         },
         {
            "time":"0930",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               }
            ]
         },
         {
            "time":"1000",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               }
            ]
         },
         {
            "time":"1030",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1100",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1130",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1200",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1230",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1300",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1330",
            "stationInfo":[
               {
                  "branchPeopleCount":0,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1400",
            "stationInfo":[
               {
                  "branchPeopleCount":2,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":2,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1430",
            "stationInfo":[
               {
                  "branchPeopleCount":2,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1500",
            "stationInfo":[
               {
                  "branchPeopleCount":2,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1530",
            "stationInfo":[
               {
                  "branchPeopleCount":2,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
         },
         {
            "time":"1600",
            "stationInfo":[
               {
                  "branchPeopleCount":2,
                  "branchStationName":"餐桌整理",
                  "branchStationCode":"124AA01",
                  "peopleInfo":[
                     {
                        "employeeEName":"TEST0608",
                        "employeePhoto":"",
                        "employeeId":"TEST0608",
                        "employeeName":"王OQ"
                     },
                     {
                        "employeeEName":"TTTT601",
                        "employeePhoto":"",
                        "employeeId":"TTTT601",
                        "employeeName":"qOq"
                     }
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"櫃台",
                  "branchStationCode":"124AA02",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"煮菜",
                  "branchStationCode":"124BB01",
                  "peopleInfo":[
                     
                  ]
               },
               {
                  "branchPeopleCount":0,
                  "branchStationName":"洗碗",
                  "branchStationCode":"124BB02",
                  "peopleInfo":[
                     
                  ]
               }
            ]
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
        "timeBlock": []
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
