# Photo
---
## 根据照片ID删除照片

```
DELETE /photos/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|照片id|

## Examples
```
localhost:3000/photos/1.json

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
