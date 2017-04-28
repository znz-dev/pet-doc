# Photo
---
## 为相簿添加照片

```
POST /photos.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|album_id|int|Y|宠物id|
|photo|file|Y|相片|

## Examples
```
localhost:3000/photos.json?album_id=3

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
    # 照片对象
    "photo": {
      # 照片ID
      "id": 1,
      # 照片url
      "photo": {
        "url": "/uploads/album/3/yellow_star.jpg"
      },
      # 照片对应的相簿ID
      "album_id": 3
    }
  }
}
```
