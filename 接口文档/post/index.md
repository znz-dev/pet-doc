# Post
---
## 查询板块帖子列表

```
GET /posts.json
```
---

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|topic_id|int|N|板块ID|
|page|int|N|页数(默认为1)|
|per|int|N|每页显示数(默认为12)|


## Examples
```
localhost:3000/posts.json?per=2&page=1&topic_id=3
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
    "posts": [
      {
        "id": 12,
        "topic_id": 3,
        "title": "设最帅",
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
