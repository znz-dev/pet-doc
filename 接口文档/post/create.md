# post
---
## 新建一个帖子

```
POST /posts.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|topic_id|int|Y|板块ID|
|user_id|int|Y|用户ID|
|title|string|Y|帖子题目|
|content|string|N|第一篇帖子回复内容|


## Examples
```
localhost:3000/posts.json?title=设最帅&topic_id=2&user_id=1&content=一楼最帅

```

## Success Response
```ruby
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "post": {
      "id": 11,
      "title": "设最帅",
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
        "id": 4,
        "content": "一楼最帅",
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
