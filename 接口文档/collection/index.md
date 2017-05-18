# Collection
---
## 查询用户全部收藏

```
GET /users/:user_id/collections.json
```
---

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|:user_id|int|Y|用户ID|
|search[resource_type]|string|N|收藏类型|
|page|int|N|页数(默认为1)|
|per|int|N|每页显示数(默认为12)|

``注：收藏类型当前可为：1. Post(帖子) 2. Pet(宠物)``
---

## Examples
```
localhost:3000/users/2/collections.json?per=2&page=1&search[resource_type]=Post
```

## Success Response
```ruby
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "total_pages": 1,
    "collections": [
      {
        "id": 30,
        "pet": {
          "id": 1,
          "name": "哈士奇",
          "species": "dog",
          "gender": "male",
          "status": null,
          "avatar": {
            "url": null
          },
          "description": null,
          "liked": 0,
          "location": null,
          "provider": {
            "id": 1,
            "username": "admin"
          },
          "adopter": null
        }
      },
      {
        "id": 32,
        "pet": {
          "id": 2,
          "name": "新小王子",
          "species": "still dog",
          "gender": "female",
          "status": null,
          "avatar": {
            "url": "/uploads/pet/avatar/2/%E8%90%A8%E6%91%A9%E8%80%B6.jpg"
          },
          "description": "我的性别？",
          "liked": 0,
          "location": null,
          "provider": {
            "id": 1,
            "username": "admin"
          },
          "adopter": {
            "id": 1,
            "username": "admin"
          }
        }
      }
    ]
  }
}
```
