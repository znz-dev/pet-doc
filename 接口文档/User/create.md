# User
---
## 新建一个用户

```
POST /users.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|username|string|Y|用户名|
|avatar|file|N|用户头像|
|password|string|Y|用户密码|
|real_name|string|N|真实姓名|
|phone|string|N|用户电话|
|email|string|N|用户邮箱|


## Examples
```
localhost:3000/users.json?username=zhangbin&password=123456&real_name=张宾&phone=18301927326&email=sbx@163.com

# 注： 传入图片的变量名为avatar
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
