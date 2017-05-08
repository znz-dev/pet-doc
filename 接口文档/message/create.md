# Message
---
## 发送消息

```
POST /messages.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|user_id|int|Y|当前用户id，即发送人id|
|receiver_id|int|Y|发送人用户id|
|content|string|Y|发送消息|

## Examples
```
localhost:3000/messages.json?user_id=3&content=lalala5&receiver_id=1

```

## Success Response
```ruby
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "message": {
      "id": 7,
      "content": "我是宾哥",
      "status": "unread",
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
  }
}
```
