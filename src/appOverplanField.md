# appOverplanField
預定加班單申請畫面欄位

### HTTP Request
```
https://114.34.125.246:8090/servlet/HRNative/appOverplanField
```

### HTTP Request Mehod
```
POST
```

### Request body
| Key | Value | Type | Description |
|:----------|:-------------|:-----|:------------|
| uid | 98599308101484732326 | String | 需透過appLogin取得
| right | 51341911904173543336756162544864820 | String | 需透過appLogin取得 |
| request | {startDate:20220526, empid:admin} | Object | 查詢條件(依據申請畫面取得)

### JSON representation
Here is a JSON representation of request.
```json
{
    "uid":"98599308101484732326",
    "right":"51341911904173543336756162544864820",
    "request":{
        "empid":"admin",
        "startDate":"20220526"  --kevin 改叫startDate
    }
}
```


### Properties
| Property | Type | Description |
|:---------|:-----|:------------|
| uid   | String | 加密後帳號 |
| right | String | 加密後系統相關資料 |
| request | Object | 要求本文 |

### Request Properties
| Key | Value | Type | Description | Required | Format |
|:----------|:-------------|:-----|:------------|:------------|:------------|
| startDate | 20220526 | String | 預定加班日期 | Y | AC(YYYYmmdd) |
| empid | admin | String | 員工編號 | Y | n/a |

### HTTP Response when Successful
```json
{
   "status":"success",
   "message":[
      "回傳成功"
   ],
   "data":{
      "overplanForm":{
         "name":"預定加班單單填寫欄位資訊",
         "type":"object",
         "value":{
            "endTime":{
               "name":"結束時間",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":true,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"string",
                     "value":"",
                     "format":"HHmm",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"endTime"
            },
            "uploadFile":{
               "name":"附件上傳",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":true,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"array",
                     "value":[
                        
                     ],
                     "format":"n/a",
                     "id":"fieldValue"
                  },
                  "uploadLimit":{
                     "name":"檔案上傳數量限制",
                     "type":"integer",
                     "value":1,
                     "format":"count",
                     "id":"uploadLimit"
                  }
               },
               "format":"n/a",
               "id":"uploadFile"
            },
            "startTime":{
               "name":"起始時間",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":true,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"string",
                     "value":"",
                     "format":"HHmm",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"startTime"
            },
            "reason":{
               "name":"加班原因",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":true,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"string",
                     "value":"",
                     "format":"n/a",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"reason"
            },
            "beforeWork":{
               "name":"跨日往前加班",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":true,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"boolean",
                     "value":false,
                     "format":"n/a",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"beforeWork"
            }
         },
         "format":"n/a",
         "id":"overplanForm"
      },
      "properties":{
         "format":{
            "HHmm":"時間時分",
            "hour":"小時",
            "YYYYmmdd":"西元年月日",
            "n/a":""
         }
      },
      "payForm":{
         "name":"給付欄位資訊",
         "type":"object",
         "value":{
            "totalRestHour":{
               "name":"總計補休時數",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":false,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"decimal",
                     "value":0.0,
                     "format":"hour",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"totalRestHour"
            },
            "payType":{
               "name":"給付方式",
               "type":"object",
               "value":{
                  "option":{
                     "name":"選項",
                     "type":"array",
                     "value":[
                        {
                           "optionId":{
                              "name":"選項代號",
                              "type":"string",
                              "value":"A",
                              "format":"n/a",
                              "id":"optionId"
                           },
                           "optionValue":{
                              "name":"選項名稱",
                              "type":"string",
                              "value":"補休",
                              "format":"n/a",
                              "id":"optionValue"
                           }
                        },
                        {
                           "optionId":{
                              "name":"選項代號",
                              "type":"string",
                              "value":"B",
                              "format":"n/a",
                              "id":"optionId"
                           },
                           "optionValue":{
                              "name":"選項名稱",
                              "type":"string",
                              "value":"給薪",
                              "format":"n/a",
                              "id":"optionValue"
                           }
                        }
                     ],
                     "format":"n/a",
                     "id":"option"
                  },
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":true,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"string",
                     "value":"B",
                     "format":"n/a",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"payType"
            },
            "totalPayHour":{
               "name":"總計給薪時數",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":false,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"decimal",
                     "value":0.0,
                     "format":"hour",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"totalPayHour"
            }
         },
         "format":"n/a",
         "id":"payForm"
      },
      "overplanInfo":{
         "name":"預定加班單單顯示欄位資訊",
         "type":"object",
         "value":{
            "empid":{
               "name":"員工編號",
               "type":"string",
               "value":"admin",
               "format":"n/a",
               "id":"empid"
            },
            "class":{
               "name":"班別",
               "type":"string",
               "value":"通用班(8-17)(0830-1730)",
               "format":"n/a",
               "id":"class"
            },
            "appliedHour":{
               "name":"當月已累積加班時數(不含本次)",
               "type":"decimal",
               "value":2.0,
               "format":"hour",
               "id":"appliedHour"
            },
            "empFullName":{
               "name":"員工中文姓名",
               "type":"string",
               "value":"系統管理員",
               "format":"n/a",
               "id":"empFullName"
            },
            "overDate":{
               "name":"加班日期",
               "type":"string",
               "value":"20220526",
               "format":"YYYYmmdd",
               "id":"overDate"
            },
            "depFullName":{
               "name":"部門名稱",
               "type":"string",
               "value":"L1線B班",
               "format":"n/a",
               "id":"depFullName"
            },
            "empFullEname":{
               "name":"員工英文姓名",
               "type":"string",
               "value":"Administrator",
               "format":"n/a",
               "id":"empFullEname"
            },
            "depCode":{
               "name":"部門代號",
               "type":"string",
               "value":"14122",
               "format":"n/a",
               "id":"depCode"
            },
            "companyFullName":{
               "name":"公司全名",
               "type":"string",
               "value":"72英特內全名(中和)",
               "format":"n/a",
               "id":"companyFullName"
            }
         },
         "format":"n/a",
         "id":"overplanInfo"
      },
      "diningForm":{
         "name":"用餐欄位資訊",
         "type":"object",
         "value":{
            "specifyHour":{
               "name":"指定時數",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":false,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"decimal",
                     "value":0.0,
                     "format":"hour",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"specifyHour"
            },
            "oldEatHour":{
               "name":"原用餐時數",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":false,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"decimal",
                     "value":0.0,
                     "format":"hour",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"oldEatHour"
            },
            "isEat":{
               "name":"是否用餐",
               "type":"object",
               "value":{
                  "fieldEditable":{
                     "name":"開放編輯",
                     "type":"boolean",
                     "value":true,
                     "format":"n/a",
                     "id":"fieldEditable"
                  },
                  "fieldValue":{
                     "name":"欄位預設值",
                     "type":"boolean",
                     "value":false,
                     "format":"n/a",
                     "id":"fieldValue"
                  }
               },
               "format":"n/a",
               "id":"isEat"
            }
         },
         "format":"n/a",
         "id":"diningForm"
      },
       "overplanTip":{  --kevin 補上備註
         "name":"預定加班單備註",
         "type":"array",
         "value":[
            {
               "name":"備註事項",
               "type":"string",
               "value":"kevinNoteTest",
               "format":"n/a",
               "id":"note"
            }
         ],
         "format":"n/a",
         "id":"overplanTip"
      }
   }
}
```

### HTTP Response when No Data
無資料則屬於 Code 500 錯誤，正常來說一般使用者一定會有資料
```json
{
    "status": "fail",
    "code": 500,
    "message": [
        "查無資料"
    ],
    "data": {}
}
```

### HTTP Response when Failed
```json
{
    "status": "fail",
    "code": 500,
    "message": [
        "XXX"
    ],
    "data": {}
}
```

### HTTP Response when Exception
```json
{
    "status": "fail",
    "code": 406,
    "message": [
        "XXX"
    ],
    "data": {}
}
```
