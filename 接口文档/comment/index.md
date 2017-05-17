# Comment
---
## 查询宠物全部留言

```
GET /pets/:pet_id/comments.json
```
---

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|:pet_id|int|Y|宠物ID|
|page|int|N|页数(默认为1)|
|per|int|N|每页显示数(默认为12)|

---

## Examples
```
localhost:3000/pets/1/comments.json?persss=1
```

## Success Response
```ruby
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "total_pages": 4,
    "comments": [
      {
        "id": 9,
        "content": "好棒",
        "created_at": "2017-05-16T15:59:22.715Z",
        "user": {
          "id": 1,
          "username": "admin",
          "avatar": {
            "url": "/uploads/user/avatar/1/yellow_star.jpg"
          }
        }
      },
      {
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
    ]
  }
}
```
