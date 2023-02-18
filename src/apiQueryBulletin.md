# apiQueryBulletin
查詢公告通知

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/shiftAPP/V1/interfaces/apiQueryBulletin
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
      "keyWord": "",
      "type": "",
      "dateItem": 1,
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
| keyWord | "" | String | 關鍵字 | n | n/a |
| dateItem | 1 | Integer | 日期項目 | n | n/a |
| type | "" | String | 選項 : 新到舊--> toOld 舊到新--> toNew 已讀--> isRead 未讀 --> unRead) | n | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| id | key值 |
| bulletinTitle | 通知主旨 |
| bulletinContent | 通知內容 |
| bulletinImg | 通知圖片 |
| announcer | 發佈者 |
| announcerImg | 發佈者圖片 |
| time | 通知時間 |
| date | 通知日期 |
| serverTime | 系統日期 |
| read | 是否已讀 |
| filesList | 檔案 |


### HTTP Response when Successful
```json
      {
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "message":"查詢成功",
      "bulletinList":[
         {
            "id":"1",
            "bulletinTitle":"推播改寫法QQ",
            "bulletinContent":"推播改寫法QQ",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"100023",
            "date":"20230214",
            "serverTime":"20230215",
            "read":true,
            "filesList":[
               
            ]
         },
         {
            "id":"3",
            "bulletinTitle":"有APP推播QQ",
            "bulletinContent":"有APP推播QQ",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"170045",
            "date":"20230214",
            "serverTime":"20230215",
            "read":true,
            "filesList":[
               
            ]
         },
         {
            "id":"14",
            "bulletinTitle":"測試多筆1",
            "bulletinContent":"測試多筆1",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171008",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"15",
            "bulletinTitle":"測試多筆2",
            "bulletinContent":"測試多筆2",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171031",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"16",
            "bulletinTitle":"測試多筆3",
            "bulletinContent":"測試多筆3",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171041",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"17",
            "bulletinTitle":"測試多筆4",
            "bulletinContent":"測試多筆4",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171052",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"18",
            "bulletinTitle":"測試多筆5",
            "bulletinContent":"測試多筆5",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171102",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"19",
            "bulletinTitle":"測試多筆6",
            "bulletinContent":"測試多筆6",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171112",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"20",
            "bulletinTitle":"測試多筆7",
            "bulletinContent":"測試多筆7",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171122",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"21",
            "bulletinTitle":"測試多筆8",
            "bulletinContent":"測試多筆8",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171130",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"22",
            "bulletinTitle":"測試多筆9",
            "bulletinContent":"測試多筆9",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171140",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"23",
            "bulletinTitle":"測試多筆10",
            "bulletinContent":"測試多筆10",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171151",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"24",
            "bulletinTitle":"英特內1",
            "bulletinContent":"英特內1",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171202",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"25",
            "bulletinTitle":"英特內2",
            "bulletinContent":"英特內2",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171226",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"26",
            "bulletinTitle":"英特內3",
            "bulletinContent":"英特內3",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171234",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"27",
            "bulletinTitle":"英特內4",
            "bulletinContent":"英特內4",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171243",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"28",
            "bulletinTitle":"英特內5",
            "bulletinContent":"英特內5",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171251",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"29",
            "bulletinTitle":"英特內6",
            "bulletinContent":"英特內6",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171259",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"30",
            "bulletinTitle":"英特內7",
            "bulletinContent":"英特內7",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171307",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"31",
            "bulletinTitle":"英特內8",
            "bulletinContent":"英特內8",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171335",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"32",
            "bulletinTitle":"英特內9",
            "bulletinContent":"英特內9",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171343",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
         },
         {
            "id":"33",
            "bulletinTitle":"英特內10",
            "bulletinContent":"英特內10",
            "bulletinImg":"",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"171352",
            "date":"20230214",
            "serverTime":"20230215",
            "read":false,
            "filesList":[
               
            ]
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
