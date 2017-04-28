# Albun
---
## 根据相簿ID查看相簿及其图片

```
GET /albums/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|相簿id|

## Examples
```
localhost:3000/albums/3.json

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
    相簿对象
    "album": {
      # 相簿ID
      "id": 3,
      # 相簿宠物ID
      "pet_id": 20,
      # 相簿描述
      "description": "萨摩耶的生活",
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
