# Post
---
## 显示指定帖子（同时显示帖子全部回复）

```
GET /posts/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|:id|int|Y|帖子ID|
|page|int|N|回复页数(默认为1)|
|per|int|N|回复每页显示数(默认为12)|


## Examples
```
localhost:3000/posts/6.json
```

## Success Response
```
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "post": {
      "id": 6,
      "topic_id": 2,
      "title": "name",
      "user": {
        "id": 1,
        "username": "admin",
        "avatar": {
          "url": "/uploads/user/avatar/1/yellow_star.jpg"
        }
      }
    },
    "reply_pages": 1,
    "post_replies": [
      {
        "id": 1,
        "content": "fdssaf",
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
