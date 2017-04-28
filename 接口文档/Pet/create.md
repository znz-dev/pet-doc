# Pet
---
## 新建一个宠物

```
POST /pets.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|name|string|Y|宠物名称|
|species|string|N|宠物品种|
|gender|string|N|宠物性别|
|status|string|N|宠物状态|
|avatar|string|N|宠物头像|
|provider_id|int|Y|宠物提供人id|
|description|string|N|宠物描述|


## Examples
```
localhost:3000/pets.json?name=小王子&species=dog&gender=male&status=1&provider_id=1

# 注： 传入图片的变量名为avatar
```

## Success Response
```ruby
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
