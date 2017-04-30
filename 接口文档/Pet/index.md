# Pet
---
## 查询全部宠物

```
GET /pets.json
```
---

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|order|string|N|排序规则(当前支持1. time_asc, 2. time_desc)|
|page|int|N|页数(默认为1)|
|per|int|N|每页显示数(默认为12)|

### 搜索参数

``参数名search[:category]``

其中，:category可选参数为
```ruby
["id", "name", "species", "gender", "status", "provider_id", "adopter_id", "created_at", "updated_at", "avatar", "description"]
```
支持的特殊搜索

1.模糊搜索

``参数名为search[like_:category]``

2.条件外搜索

``参数名为search[not_:category]``


---

## Examples
```
120.25.124.236:3000/pets.json?per=2&page=1&order=time_desc
```

## Success Response
```ruby
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    # 宠物数组对象，其中的每一个子对象介绍参考create.md
    "pets": [
      {
        "id": 13,
        "name": "哈士奇",
        "species": "dog",
        "gender": "male",
        "status": null,
        "avatar": {
          "url": "/uploads/pet/avatar/13/%E5%93%88%E5%A3%AB%E5%A5%87.jpg"
        },
        "description": null,
        "provider": {
          "id": 1,
          "username": "zhouxin"
        },
        "adopter": null
      },
      {
        "id": 14,
        "name": "布偶猫",
        "species": "cat",
        "gender": "female",
        "status": null,
        "avatar": {
          "url": "/uploads/pet/avatar/14/%E5%B8%83%E5%81%B6%E7%8C%ABjpg"
        },
        "description": null,
        "provider": {
          "id": 1,
          "username": "zhouxin"
        },
        "adopter": null
      },
      {
        "id": 15,
        "name": "挪威森林猫",
        "species": "cat",
        "gender": "male",
        "status": null,
        "avatar": {
          "url": "/uploads/pet/avatar/15/%E6%8C%AA%E5%A8%81%E6%A3%AE%E6%9E%97%E7%8C%AB.jpg"
        },
        "description": null,
        "provider": {
          "id": 1,
          "username": "zhouxin"
        },
        "adopter": null
      }
    ]
  }
}
```
