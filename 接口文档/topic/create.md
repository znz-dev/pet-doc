# topic
---
## 新建一个板块

```
POST /topics.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|name|string|Y|板块名称|
|avatar|string|Y|板块头像|
|description|string|N|板块描述|


## Examples
```
localhost:3000/topics.json?name=萌宠大作战1&description=呼呼压抑

# 注： 传入图片的变量名为avatar
```

## Success Response
```ruby
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "topic": {
      "id": 3,
      "name": "萌宠大作战1",
      "avatar": {
        "url": null
      },
      "description": "呼呼压抑"
    }
  }
}
```
