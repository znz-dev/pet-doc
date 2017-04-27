# Pet
---
## 新建一个宠物

```
POST /pets.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|name|string|Y|宠物名称|
|species|string|N|宠物品种|
|gender|string|N|宠物性别|
|status|string|N|宠物状态|
|avatar|string|N|宠物头像|
|provider_id|int|Y|宠物提供人id|


## Examples
```
localhost:3000/pets.json?name=希尔哇纳斯&species=cat&gender=female&status=1&provider_id=1

# 注： 传入图片的变量名为avatar
```

## Success Response
```ruby
{
  "status": {
    # 接口返回状态
    "code": "20000",
    "message": ""
  },
  "data": {
    # 宠物ID
    "id": 5,
    # 宠物姓名
    "name": "希尔哇纳斯",
    # 宠物物种
    "species": "cat",
    # 宠物性别
    "gender": "female",
    # 暂时不用
    "status": "1",
    # 头像
    "avatar": {
      "url": "/uploads/pet/avatar/5/yellow_star.jpg"
    },
    # 宠物提供人信息
    "provider": {
      "id": 1,
      "username": "zhouxin"
    }
    # 宠物收养人信息,如果为空，则该宠物没有收养人，如果宠物有收养人，那么格式和提供人相同。
    "adopter": null
  }
}
```
