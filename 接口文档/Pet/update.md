# Pet
---
## 更新宠物信息

```
PUT /pets/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|name|string|N|宠物名称|
|species|string|N|宠物品种|
|gender|string|N|宠物性别|
|status|string|N|宠物状态|
|avatar|file|N|宠物头像文件|


## Examples
```
localhost:3000/pets/22.json?name=新小王子&species=still dog&gender=female&description=我的性别？&adopter_id=1

# 注： 传入图片的变量名为avatar
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
      "name": "新小王子",
      # 宠物品种
      "species": "still dog",
      # 宠物性别
      "gender": "female",
      # 宠物状态
      "status": "1",
      # 宠物头像
      "avatar": {
        "url": "/uploads/pet/avatar/22/%E8%90%A8%E6%91%A9%E8%80%B6.jpg"
      },
      # 宠物描述
      "description": "我的性别？",
      # 宠物提供人
      "provider": {
        "id": 1,
        "username": "zhouxin"
      },
      # 宠物领养人，根据判断是不是Null来确定是不是已领养
      "adopter": {
        "id": 1,
        "username": "zhouxin"
      }
    }
  }
}

```
