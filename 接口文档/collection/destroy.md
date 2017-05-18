# Collection
---
## 删除收藏

```
DELETE /collections/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|:id|int|Y|收藏ID|


## Examples
```
localhost:3000/collections/27.json
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
