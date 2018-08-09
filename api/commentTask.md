# （用  户）评价: commentTask

- 订单完成，用户对设计师评价

## 参数

    {
        'id': // 订单ID
        'designer_id': // 设计师ID
        'service_score': Int, // 服务分数
        'design_score': Int, // 设计分数
        'comment': String // 评价详情
    }

## 返回数据

    {
        "message": "评价成功!",
        "status": 200
    }

## 说明

- 用户评价成功给与积分奖励，多少由后台配置
