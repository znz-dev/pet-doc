# Message
---
## 根据消息ID查看消息

``注： 如果当前用户是收信人，那么调用次接口会自动将信息状态变更为已读``

```
GET /messages/:id.json

```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|user_id|int|Y|当前用户id|

## Examples
```
localhost:3000/messages/7.json?user_id=1

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
  }
}
```
