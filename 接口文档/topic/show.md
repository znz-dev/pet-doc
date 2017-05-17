# Topic
---
## 显示指定板块

```
GET /topics/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|:id|int|Y|板块ID|


## Examples
```
localhost:3000/topics/3.json
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
      "name": "萌宠大作战1",
      "avatar": {
        "url": null
      },
      "description": "呼呼压抑"
    }
  }
}
```
