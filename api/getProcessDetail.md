# 查看订单进度详情: getProcessDetail

- 查看订单的进度详情

## 参数

    {
        "task_id": // 订单ID
        "designer_id": // 设计师ID
    }

## 返回数据

    {
        "process_list": [ // 进度列表：初稿，支付、审核、终稿、凭证等
            {
                "process_"
                "explain": // 设计描述
                "part": // 房间名称
            },
            // ...
        ],
        "3d_url": // 3d案例的链接
        "explain": // 设计说明
        "message": "获取数据成功!",
        "status": 200
    }
