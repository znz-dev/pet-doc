# Pet
---
## 显示指定宠物

```
GET /pets/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|宠物id|


## Examples
```
localhost:3000/pets/6.json
```

## Success Response
```
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "id": 6,
    "name": "希尔哇纳斯",
    "species": "cat",
    "gender": "female",
    "status": "1",
    "avatar": {
      "url": "/uploads/pet/avatar/6/yellow_star.jpg"
    },
    "provider": {
      "id": 1,
      "username": "zhouxin"
    }
  }
}
```
