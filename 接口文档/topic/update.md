# Pet
---
## 更新宠物信息

```
PUT /comments/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|name|string|Y|板块名称|
|avatar|string|Y|板块头像|
|description|string|N|板块描述|
|:id|int|Y|板块ID|


## Examples
```
localhost:3000/pets/22.json?name=新小王子&species=still dog&gender=female&description=我的性别？&adopter_id=1

# 注： 传入图片的变量名为avatar
```

## Success Response
```
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "topic": {
      "id": 3,
      "name": "萌宠作战第二部",
      "avatar": {
        "url": "/uploads/topic/avatar/3/yellow_star.jpg"
      },
      "description": "呼呼压抑cuod大大的a"
    }
  }
}

```
