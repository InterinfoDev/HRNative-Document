# appWorkPlace
取得使用者上班地點資訊

### HTTP Request
```
https://114.34.125.246:8090/servlet/HRNative/appWorkPlace
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


### JSON representation
Here is a JSON representation of request.
```json
{
   "uid":"98599308101484732326",
   "right":"51341911904173543336756162544864820",
}
```

### Properties
| Property | Type | Description |
|:---------|:-----|:------------|
| uid   | String | 加密後帳號 |
| right | String | 加密後系統相關資料 |

### HTTP Response when Successful
```json
{
   "status":"success",
   "message":[
      "回傳成功"
   ],
   "data":{
      "properties":{
         "format":{
            "n/a":"",
            "meter":"公尺"
         }
      },
      "workPlaceList":{
         "name":"工作地點清單",
         "type":"array",
         "value":[
            {
               "name":"工作地點資訊",
               "type":"object",
               "value":{
                  "radius":{
                     "name":"打卡半徑",
                     "type":"decimal",
                     "value":7.0,
                     "format":"meter",
                     "id":"radius"
                  },
                  "location":{
                     "name":"工作位置",
                     "type":"decimal",
                     "value":{
                        "longitude":{
                           "name":"經度",
                           "type":"decimal",
                           "value":23.883403,
                           "format":"n/a",
                           "id":"longitude"
                        },
                        "latitude":{
                           "name":"緯度",
                           "type":"decimal",
                           "value":120.945517,
                           "format":"n/a",
                           "id":"latitude"
                        }
                     },
                     "format":"meter",
                     "id":"location"
                  },
                  "placeName":{
                     "name":"工作地點中文名稱",
                     "type":"string",
                     "value":"澎湖",
                     "format":"n/a",
                     "id":"placeName"
                  },
                  "placeEname":{
                     "name":"工作地點英文名稱",
                     "type":"string",
                     "value":"",
                     "format":"n/a",
                     "id":"placeEname"
                  },
                  "placeCode":{
                     "name":"工作地點代號",
                     "type":"string",
                     "value":"TW19",
                     "format":"n/a",
                     "id":"placeCode"
                  }
               },
               "format":"n/a",
               "id":"workPlace"
            },
            {
               "name":"工作地點資訊",
               "type":"object",
               "value":{
                  "radius":{
                     "name":"打卡半徑",
                     "type":"decimal",
                     "value":7.0,
                     "format":"meter",
                     "id":"radius"
                  },
                  "location":{
                     "name":"工作位置",
                     "type":"decimal",
                     "value":{
                        "longitude":{
                           "name":"經度",
                           "type":"decimal",
                           "value":25.0338,
                           "format":"n/a",
                           "id":"longitude"
                        },
                        "latitude":{
                           "name":"緯度",
                           "type":"decimal",
                           "value":121.5645,
                           "format":"n/a",
                           "id":"latitude"
                        }
                     },
                     "format":"meter",
                     "id":"location"
                  },
                  "placeName":{
                     "name":"工作地點中文名稱",
                     "type":"string",
                     "value":"澎湖",
                     "format":"n/a",
                     "id":"placeName"
                  },
                  "placeEname":{
                     "name":"工作地點英文名稱",
                     "type":"string",
                     "value":"",
                     "format":"n/a",
                     "id":"placeEname"
                  },
                  "placeCode":{
                     "name":"工作地點代號",
                     "type":"string",
                     "value":"TW19",
                     "format":"n/a",
                     "id":"placeCode"
                  }
               },
               "format":"n/a",
               "id":"workPlace"
            }
         ],
         "format":"n/a",
         "id":"workPlaceList"
      }
   }
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
