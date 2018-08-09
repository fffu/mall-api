# （设计师）提交方案: commitDraft

- 设计师提交设计方案

## 参数

    {
        'id': // 订单ID
        'solution': [//方案
            {
                'image_id': // 图片ID
                'explain': // 设计描述
            },
            // ...
        ],
        '3d_url': // 3d案例的链接
        'explain': // 设计说明
        'process_id': // 进度ID
        'type': // 1为初稿、2为终稿、3为上传设计师自己案例
    }

## 返回数据

    {
        "message": "提交*稿成功!",
        "status": 200
    }


## 说明

- 提交设计稿给予设计师积分奖励，多少由后台配置