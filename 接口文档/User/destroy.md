# User
---
## 删除用户

```
DELETE /users/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|用户id|


## Examples
```
localhost:3000/users/2.json
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
