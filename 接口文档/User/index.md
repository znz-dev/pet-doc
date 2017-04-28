# User
---
## 查询全部用户

```
GET /users.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|page|int|N|页数(默认为1)|
|per|int|N|每页显示数(默认为12)|


## Examples
```
localhost:3000/users.json?page=2&per=1
```

## Success Response
```ruby
{
  "status": {
    # 状态码
    "code": "20000",
    "message": ""
  },
  "data": {
    # 用户数组对象
    "users": [
      {
        # 用户ID
        "id": 3,
        # 用户名
        "username": "zhangbin",
        # 用户真实姓名
        "real_name": "张宾",
        # 用户手机号码
        "phone": "18301927326",
        # 用户邮箱号码
        "email": "sbx@163.com"
      }
    ]
  }
}
```
