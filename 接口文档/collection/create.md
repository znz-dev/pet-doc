# Collection (收藏)
---
## 新建一个收藏

```
POST /collections.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|resource_type|string|Y|收藏类型|
|resource_id|int|Y|收藏ID|
|user_id|int|Y|用户ID|

``注：收藏类型当前可为：1. Post(帖子) 2. Pet(宠物)``
---

## Examples
```
localhost:3000/collections.json?resource_type=Post&resource_id=1&user_id=2

```

## Success Response
```ruby
{
  "status": {
    "code": "50000",
    "message": "Validation failed: Resource 你已经收藏过了"
  },
  "data": {
    "collection": {
      "id": null,
      "post": {
        "id": 1,
        "topic_id": 2,
        "title": "name",
        "created_at": "2017-05-17T06:42:56.951Z",
        "user": {
          "id": 1,
          "username": "admin",
          "avatar": {
            "url": "/uploads/user/avatar/1/yellow_star.jpg"
          }
        }
      }
    }
  }
}
```
