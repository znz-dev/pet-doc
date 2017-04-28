# Pet
---
## 查询全部宠物

```
GET /pets.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|order|string|N|排序规则(当前支持1. time_asc, 2. time_desc)|
|page|int|N|页数(默认为1)|
|per|int|N|每页显示数(默认为12)|


## Examples
```
120.25.124.236:3000/pets.json?per=2&page=1&order=time_desc
```

## Success Response
```
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": [
    {
      "id": 8,
      "name": "萨摩耶",
      "species": "dog",
      "gender": "female",
      "status": null,
      "avatar": {
        "url": "/uploads/pet/avatar/8/%E8%90%A8%E6%91%A9%E8%80%B6.jpg"
      },
      "provider": {
        "id": 1,
        "username": "zhouxin"
      },
      "adopter": null
    },
    {
      "id": 7,
      "name": "英国短毛猫",
      "species": "cat",
      "gender": "male",
      "status": null,
      "avatar": {
        "url": null
      },
      "provider": {
        "id": 1,
        "username": "zhouxin"
      },
      "adopter": null
    }
  ]
}
```
