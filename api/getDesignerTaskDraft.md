# （设计师）查看订单设计详情: getDesignerTaskDraft

- 设计师查看自己提交的方案

## 参数

    {
        'process_id': // 进度ID
        'order_id': // 订单ID
    }

## 返回数据

    {
        {
            'solution': [//提交方案详情
                {
                    'image':{
                        'small_path': String, // 图片路径
                        'medium_path': String, // 图片路径
                        'big_path': String, // 图片路径
                    }
                    'explain': // 设计描述
                    'part': //房间名称
                },
                // ...
            ],
            '3d_url': // 3d案例的链接
            'explain': // 设计说明
        },
        "message": "获取详情成功!",
        "status": 200
    }
