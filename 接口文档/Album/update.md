# Album
---
## 更新相簿信息

```
PUT /albums/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|pet_id|int|N|宠物id|
|description|string|N|相簿描述|


## Examples
```
localhost:3000/albums/:id.json?description=新的描述

# 注： 传入图片的变量名为avatar
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
    相簿对象
    "album": {
      # 相簿ID
      "id": 3,
      # 相簿宠物ID
      "pet_id": 20,
      # 相簿描述
      "description": "新的描述",
      # 相簿相片数组对象
      "photos": [
        {
          # 照片ID
          "id": 2,
          # 照片URL
          "photo": {
            "url": "/uploads/album/3/%E8%90%A8%E6%91%A9%E8%80%B6.jpg"
          }
        },
        {
          "id": 3,
          "photo": {
            "url": "/uploads/album/3/%E7%BC%85%E5%9B%A0%E7%8C%AB.jpg"
          }
        }
      ]
    }
  }
}

```
