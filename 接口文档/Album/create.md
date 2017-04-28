# Album
---
## 新建一个宠物相簿

```
POST /albums.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|pet_id|int|Y|宠物id|
|description|string|N|相簿描述|

## Examples
```
localhost:3000/albums.json?description=萨摩耶的生活&pet_id=20

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
    # 相簿对象
    "album": {
      # 相簿ID
      "id": 3,
      # 相簿对应的宠物ID
      "pet_id": 20,
      # 相簿描述
      "description": "萨摩耶的生活",
      # 相簿中的照片数组，由于是新建相簿，那么，相簿里面还没有照片
      "photos": []
    }
  }
}
```
