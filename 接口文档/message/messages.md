# Message
---
## 用户查看自己的消息(默认返回所有发送消息和接收消息)

```
GET /users/:user_id/messages

```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|user_id|int|Y|当前用户id|

## Examples
```
localhost:3000/users/1/messages?search[receiver_id]=1

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
    "messages": [
      {
        "id": 6,
        "content": "lalala5",
        "status": "unread",
        "created_at": "2017-05-08T06:29:01.477Z",
        "sender": {
          "id": 3,
          "username": "zhangbin"
        },
        "receiver": {
          "id": 1,
          "username": "zhouxin"
        }
      },
      {
        "id": 7,
        "content": "我是宾哥",
        "status": "readed",
        "created_at": "2017-05-08T06:37:46.372Z",
        "sender": {
          "id": 3,
          "username": "zhangbin"
        },
        "receiver": {
          "id": 1,
          "username": "zhouxin"
        }
      }
    ]
  }
}
```
