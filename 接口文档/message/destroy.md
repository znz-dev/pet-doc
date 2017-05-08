# Message
---
## 根据消息ID删除消息

```
DELETE /messages/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|照片id|

## Examples
```
localhost:3000/messages/2.json

```

## Success Response
```ruby
{
  "status": {
    # 状态码
    "code": "20000",
    "message": ""
  },
  "data": {}
}
```
