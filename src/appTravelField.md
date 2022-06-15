# appTravelField
出差單申請畫面欄位

### HTTP Request
```
https://114.34.125.246:8090/servlet/HRNative/appTravelField
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
| request | {empid:admin} | Object | 查詢條件(依據申請畫面取得，加班日期與預定加班單號只可擇一輸入)

### JSON representation
Here is a JSON representation of request.
```json
{
    "uid":"98599308101484732326",
    "right":"51341911904173543336756162544864820",
    "request":{
        "empid":"admin",
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
| empid | admin | String | 員工編號 | Y | n/a |

### HTTP Response when Successful
```json
{
    "status": "success",
    "message": [
        "回傳成功"
    ],
    "data": {
        "travelTip": {
            "name": "出差單備註",
            "type": "array",
            "value": [],
            "format": "n/a",
            "id": "travelTip"
        },
        "properties": {
            "format": {
                "HHmm": "時間時分",
                "currency": "元",
                "YYYYmmdd": "西元年月日",
                "n/a": ""
            }
        },
        "applyForm": {
            "name": "出差單填寫欄位資訊",
            "type": "object",
            "value": {
                "point": {
                    "name": "備註",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "note"
                },
                "contact": {
                    "name": "備註",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "note"
                },
                "visit": {
                    "name": "備註",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "note"
                },
                "people": {
                    "name": "備註",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "note"
                },
                "uploadFile": {
                    "name": "附件上傳",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "array",
                            "value": [],
                            "format": "n/a",
                            "id": "fieldValue"
                        },
                        "uploadLimit": {
                            "name": "檔案上傳數量限制",
                            "type": "integer",
                            "value": 3,
                            "format": "count",
                            "id": "uploadLimit"
                        }
                    },
                    "format": "n/a",
                    "id": "uploadFile"
                },
                "authorize": {
                    "name": "備註",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "note"
                },
                "assist": {
                    "name": "備註",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "note"
                },
                "schedule": {
                    "name": "備註",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "note"
                }
            },
            "format": "n/a",
            "id": "applyForm"
        },
        "travelForm": {
            "name": "出差單填寫欄位資訊",
            "type": "object",
            "value": {
                "flowAgent3": {
                    "name": "代理人三",
                    "type": "object",
                    "value": {
                        "option": {
                            "name": "選項",
                            "type": "array",
                            "value": [
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "10900015",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "2O3",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                }
                            ],
                            "format": "n/a",
                            "id": "option"
                        },
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": false,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "flowAgent3"
                },
                "flowAgent2": {
                    "name": "代理人二",
                    "type": "object",
                    "value": {
                        "option": {
                            "name": "選項",
                            "type": "array",
                            "value": [
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "10900015",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "2O3",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                }
                            ],
                            "format": "n/a",
                            "id": "option"
                        },
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": false,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "flowAgent2"
                },
                "flowAgent1": {
                    "name": "代理人一",
                    "type": "object",
                    "value": {
                        "option": {
                            "name": "選項",
                            "type": "array",
                            "value": [
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "10900015",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "2O3",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                }
                            ],
                            "format": "n/a",
                            "id": "option"
                        },
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": false,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "flowAgent1"
                },
                "startTime": {
                    "name": "起始時間",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "0800",
                            "format": "HHmm",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "startTime"
                },
                "startDate": {
                    "name": "起始日期",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "20220615",
                            "format": "YYYYmmdd",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "startDate"
                },
                "travelPlace": {
                    "name": "出差地點",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "travelPlace"
                },
                "traffic": {
                    "name": "交通工具",
                    "type": "object",
                    "value": {
                        "option": {
                            "name": "選項",
                            "type": "array",
                            "value": [
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "1",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "捷運",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "2",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "火車",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "3",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "公車／客運",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "4",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "公務車",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "5",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "私用車",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "6",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "飛機",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "7",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "機車",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "8",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "計程車",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "9",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "高鐵",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "0",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "其它",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                }
                            ],
                            "format": "n/a",
                            "id": "option"
                        },
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": "true",
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "traffic"
                },
                "travelType": {
                    "name": "出差類別",
                    "type": "object",
                    "value": {
                        "option": {
                            "name": "選項",
                            "type": "array",
                            "value": [],
                            "format": "n/a",
                            "id": "option"
                        },
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": "true",
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "travelType"
                },
                "jobAgent": {
                    "name": "職務代理人",
                    "type": "object",
                    "value": {
                        "option": {
                            "name": "選項",
                            "type": "array",
                            "value": [
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "10900015",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "2O3",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                }
                            ],
                            "format": "n/a",
                            "id": "option"
                        },
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "10900015",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "jobAgent"
                },
                "preCost": {
                    "name": "預支旅費",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "integer",
                            "value": "0",
                            "format": "currency",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "preCost"
                },
                "endDate": {
                    "name": "結束日期",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "20220615",
                            "format": "YYYYmmdd",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "endDate"
                },
                "endTime": {
                    "name": "結束時間",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "1700",
                            "format": "HHmm",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "endTime"
                },
                "flowAgent": {
                    "name": "簽核代理人",
                    "type": "object",
                    "value": {
                        "option": {
                            "name": "選項",
                            "type": "array",
                            "value": [
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "10900015",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "2O3",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                }
                            ],
                            "format": "n/a",
                            "id": "option"
                        },
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "10900015",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "flowAgent"
                },
                "note": {
                    "name": "備註",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "note"
                },
                "currency": {
                    "name": "幣別",
                    "type": "object",
                    "value": {
                        "option": {
                            "name": "選項",
                            "type": "array",
                            "value": [
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "HK",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "港幣",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "JPY",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "日幣",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "NTD",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "台幣",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "RMB",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "人民幣",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "SGD",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "新加坡幣",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "USD",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "美元",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                },
                                {
                                    "optionId": {
                                        "name": "選項代號",
                                        "type": "string",
                                        "value": "VND",
                                        "format": "n/a",
                                        "id": "optionId"
                                    },
                                    "optionValue": {
                                        "name": "選項名稱",
                                        "type": "string",
                                        "value": "越南幣",
                                        "format": "n/a",
                                        "id": "optionValue"
                                    }
                                }
                            ],
                            "format": "n/a",
                            "id": "option"
                        },
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": "true",
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "string",
                            "value": "",
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "currency"
                },
                "isHoliday": {
                    "name": "是否包含假日",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "boolean",
                            "value": false,
                            "format": "n/a",
                            "id": "fieldValue"
                        }
                    },
                    "format": "n/a",
                    "id": "isHoliday"
                },
                "uploadFile": {
                    "name": "附件上傳",
                    "type": "object",
                    "value": {
                        "fieldEditable": {
                            "name": "開放編輯",
                            "type": "boolean",
                            "value": true,
                            "format": "n/a",
                            "id": "fieldEditable"
                        },
                        "fieldValue": {
                            "name": "欄位預設值",
                            "type": "array",
                            "value": [],
                            "format": "n/a",
                            "id": "fieldValue"
                        },
                        "uploadLimit": {
                            "name": "檔案上傳數量限制",
                            "type": "integer",
                            "value": 1,
                            "format": "count",
                            "id": "uploadLimit"
                        }
                    },
                    "format": "n/a",
                    "id": "uploadFile"
                }
            },
            "format": "n/a",
            "id": "travelForm"
        },
        "travelInfo": {
            "name": "出差單顯示欄位資訊",
            "type": "object",
            "value": {
                "depCode": {
                    "name": "部門代號",
                    "type": "string",
                    "value": "99999",
                    "format": "n/a",
                    "id": "depCode"
                },
                "applyDate": {
                    "name": "申請日期",
                    "type": "string",
                    "value": "英特內股份有限公司",
                    "format": "n/a",
                    "id": "applyDate"
                },
                "companyFullName": {
                    "name": "公司全名",
                    "type": "string",
                    "value": "72英特內全名(中和)",
                    "format": "n/a",
                    "id": "companyFullName"
                },
                "empFullName": {
                    "name": "員工中文姓名",
                    "type": "string",
                    "value": "系統管理員",
                    "format": "n/a",
                    "id": "empFullName"
                },
                "empid": {
                    "name": "員工編號",
                    "type": "string",
                    "value": "admin",
                    "format": "n/a",
                    "id": "empid"
                },
                "depFullName": {
                    "name": "部門名稱",
                    "type": "string",
                    "value": "英特內股份有限公司",
                    "format": "n/a",
                    "id": "depFullName"
                }
            },
            "format": "n/a",
            "id": "travelInfo"
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