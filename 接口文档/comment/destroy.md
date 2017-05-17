# Comment
---
## 删除留言

```
DELETE /comments/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|留言ID|


## Examples
```
localhost:3000/comments/1.json
```

## Success Response
```
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {}
}
```
