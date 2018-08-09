# （公  司）审核设计师的设计: reviewDraft

## 参数

    {
        'process_id': // 进度id
        'ispass': Int // 1通过，2不通过
        'explain': String // 处理说明
    }

## 返回数据

    {
        "message": "操作成功!",
        "status": 200
    }

## 说明

- 需要判断公司权限
- 最后施工图审核通过后订单完结，给予公司积分奖励，多少由平台配置