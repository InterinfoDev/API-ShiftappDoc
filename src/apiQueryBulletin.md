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
      "bulletinCount": 10,
      "keyWord": "",
      "lastKey": "8" ,
      "type": "" 
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
| bulletinCount | 10 | Integer | 顯示筆數 | n | n/a |
| keyWord | "" | String | 關鍵字 | n | n/a |
| lastKey | "8" | Integer | 最後筆數 | n | n/a |
| type | "" | Integer | 選項 : 新到舊--> toOld 舊到新--> toNew 已讀--> isRead 未讀 --> unRead) | n | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| id | key值 |
| bulletinTitle | 通知主旨 |
| bulletinContent | 通知內容 |
| announcer | 發佈者 |
| announcerImg | 發佈者圖片 |
| time | 通知時間 |
| date | 通知日期 |
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
            "id":"9",
            "bulletinTitle":"測試6",
            "bulletinContent":"測試6",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"170443",
            "date":"20230210",
            "read":false,
            "filesList":[
               {
                  "filesKey":"3686482232372505193311491069793949974906302509533992293460953544329316936301903569805892690000059981550238049811264662440285101131861365",
                  "fileName":"1676019901359_catty1.htm"
               },
               {
                  "filesKey":"68003594272853068328215665708396536910803200539809124725653221089541935775145452683263577481564575505235792937421566485926408642117458655667740378798954939",
                  "fileName":"1676019901361_suitespotlogo.gif"
               }
            ]
         },
         {
            "id":"10",
            "bulletinTitle":"測試7",
            "bulletinContent":"測試7",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"170501",
            "date":"20230210",
            "read":false,
            "filesList":[
               {
                  "filesKey":"68003594272853068328215665708396536910803200539809124725653221089541935775145524184110891640206309849729206713051762127048046300522499030472694301001047559",
                  "fileName":"1676019921620_hrm8w_kanpai.htm"
               },
               {
                  "filesKey":"1254444899643701143193487589634957007592993216761018430885254943967499105724802120184748470458723888959045356635906134050589192281814116870911070921963019284651790204544267438",
                  "fileName":"1676019921621_1535358729459_A02.jpg"
               }
            ]
         },
         {
            "id":"11",
            "bulletinTitle":"測試8",
            "bulletinContent":"測試8",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"170522",
            "date":"20230210",
            "read":false,
            "filesList":[
               {
                  "filesKey":"68003594272853068328215665708396536910803200539809124725653221089541935775145443631223028540985516435798085854961150392249426776692572237316159627056256938",
                  "fileName":"1676019940515_hrm8b_walsin3.html"
               },
               {
                  "filesKey":"1254444899643701143193487589634957007592993216761018430885254943967499105724800634246241661643105587655084434488783526257742557956513421329960077602744717632622694615111593130",
                  "fileName":"1676019940516_Resume_BackGround.jpg"
               }
            ]
         },
         {
            "id":"12",
            "bulletinTitle":"測試9",
            "bulletinContent":"測試9",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"170541",
            "date":"20230210",
            "read":false,
            "filesList":[
               {
                  "filesKey":"68003594272853068328215665708396536910803200539809124725653221089541935775145512591452578974795585766937412772418672899192952520539333198496666129014270268",
                  "fileName":"1676019957890_indexintabel.htm"
               },
               {
                  "filesKey":"3686482232372505193311491069793949974906302509533992293460953544329316936301906817435325944558245086789505036920536616322311603270254573",
                  "fileName":"1676019957893_綠燈.jpg"
               }
            ]
         },
         {
            "id":"13",
            "bulletinTitle":"測試10",
            "bulletinContent":"測試10",
            "announcer":"admin",
            "announcerImg":"http://59.124.100.151:8090/servlet/jform?em_step=2&file=hrm8w.pkg&enc=93d23f3a4b3f18574d52104f57504b50100e09080a0e0b070e0e0d09080d606c60600b0e0d090c0e0f0911554f58",
            "time":"170558",
            "date":"20230210",
            "read":false,
            "filesList":[
               {
                  "filesKey":"3686482232372505193311491069793949974906302509533992293460953544329316936301906246809703664703440817647325235966512687303884498841415329",
                  "fileName":"1676019977763_emaker.htm"
               },
               {
                  "filesKey":"3686482232372505193311491069793949974906302509533992293460953544329316936301906246809703664703440945168832333643770569628840064523362077",
                  "fileName":"1676019977764_STOP.png"
               }
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
