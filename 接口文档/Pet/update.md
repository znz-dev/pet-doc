# Pet
---
## 新建一个宠物

```
PUT /pets/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|name|string|N|宠物名称|
|species|string|N|宠物品种|
|gender|string|N|宠物性别|
|status|string|N|宠物状态|
|avatar|string|N|宠物头像|


## Examples
```
localhost:3000/pets/6.json?name=金色希尔哇纳斯&species=dog&gender=male&status=1

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
    "id": 6,
    "name": "金色希尔哇纳斯",
    "species": "dog",
    "gender": "male",
    "status": "1",
    "avatar": {
      "url": null
    },
    "provider": {
      "id": 1,
      "username": "zhouxin"
    }
  }
}

```
