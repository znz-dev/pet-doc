# Post
---
## 删除帖子

```
DELETE /posts/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|:id|int|Y|帖子ID|


## Examples
```
localhost:3000/posts/7.json
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
