# Topic
---
## 查询全部全部板块

```
GET /topics.json
```
---

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|


## Examples
```
localhost:3000/topics.json?
```

## Success Response
```ruby
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {
    "topics": [
      {
        "id": 2,
        "name": "萌宠大作战",
        "avatar": {
          "url": null
        },
        "description": "呼呼压抑"
      },
      {
        "id": 3,
        "name": "萌宠大作战1",
        "avatar": {
          "url": null
        },
        "description": "呼呼压抑"
      }
    ]
  }
}
```
