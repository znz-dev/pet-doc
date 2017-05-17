# Topic
---
## 删除板块

```
DELETE /topics/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|:id|int|Y|板块ID|


## Examples
```
localhost:3000/topics/3.json
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
