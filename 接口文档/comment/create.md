# Comment（留言板）
---
## 新建一个宠物

```
POST /comments.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|user_id|string|Y|用户ID|
|pet_id|string|Y|宠物ID|
|content|string|Y|留言内容|


## Examples
```
localhost:3000/comments.json?user_id=1&pet_id=1&content=你好漂亮

```

## Success Response
```ruby
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "comment": {
      "id": 10,
      "content": "你好漂亮",
      "created_at": "2017-05-17T01:37:26.217Z",
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
```
