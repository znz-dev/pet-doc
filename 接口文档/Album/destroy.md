# Album
---
## 根据相簿ID删除相簿

```
DELETE /albums/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|相簿id|

## Examples
```
localhost:3000/albums/3.json

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
