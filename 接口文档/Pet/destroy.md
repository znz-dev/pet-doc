# Pet
---
## 删除宠物

```
DELETE /pets/:id.json
```

## Parameters

|参数名|参数类型|是否必填|参数描述|
|-----|--------|-------|--------|
|id|int|Y|宠物id|


## Examples
```
localhost:3000/pets/6.json
```

## Success Response
```
{
  "status": {
    "code": "20000",
    "message": ""
  },
  "data": {}
}
```
