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
localhost:3000/pets/22.json
```

## Success Response
```
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    # 宠物对象
    "pet": {
      # 宠物ID
      "id": 22,
      # 宠物名
      "name": "小王子",
      # 宠物品种
      "species": "dog",
      # 宠物性别
      "gender": "male",
      # 宠物状态
      "status": "1",
      # 宠物头像
      "avatar": {
        "url": "/uploads/pet/avatar/22/yellow_star.jpg"
      },
      # 宠物描述
      "description": "我是小王子",
      # 宠物提供人
      "provider": {
        "id": 1,
        "username": "zhouxin"
      },
      # 宠物领养人，根据判断是不是Null来确定是不是已领养
      "adopter": null
    }
  }
}
```
