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
localhost:3000/pets.json?order=time_asc
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
      "id": 3,
      "name": "妞妞",
      "species": "dog",
      "gender": "female",
      "status": "1",
      "avatar": {
        "url": null
      },
      "provider": {
        "id": 1,
        "username": "zhouxin"
      }
    },
    {
      "id": 4,
      "name": "端午",
      "species": "cat",
      "gender": "female",
      "status": "1",
      "avatar": {
        "url": null
      },
      "provider": {
        "id": 1,
        "username": "zhouxin"
      }
    },
    {
      "id": 5,
      "name": "希尔哇纳斯",
      "species": "cat",
      "gender": "female",
      "status": "1",
      "avatar": {
        "url": "/uploads/pet/avatar/5/yellow_star.jpg"
      },
      "provider": {
        "id": 1,
        "username": "zhouxin"
      }
    }
  ]
}
```
