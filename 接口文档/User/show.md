# User
---
## 显示指定用户

```
GET /users/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|用户ID|


## Examples
```
localhost:3000/users/3.json
```

## Success Response
```
{
  "status": {
    # 状态码
    "code": "20000",
    "message": ""
  },
  "data": {
    # 用户对象
    "user": {
      # 用户id
      "id": 3,
      # 用户名
      "username": "zhangbin",
      # 用户真实姓名
      "real_name": "张宾",
      # 用户手机
      "phone": "18301927326",
      # 用户邮箱
      "email": "sbx@163.com"
    }
  }
}
```
