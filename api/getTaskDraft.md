# （用  户）查看订单设计详情: getTaskDraft

- 用户个人中心查看设计师提交的方案

## 参数

    {
        'id': //
        'process_type': // 0：初稿；1：终稿；2：施工图
    }

## 返回数据

    {
        'content': [
            {
                'processID': //
                'designerID': //
                'designer_name': //
                '3durl': //
                'explain': //
                'solution': [
                    {
                        'image':{
                            'sml': String, // 图片路径
                            'mid': String, // 图片路径
                            'big': String, // 图片路径
                            'ori': String, // 图片路径
                        }
                        'part_name': // 房间名称
                        'explain': // 设计描述
                    },
                    // ...
                ],
                'examine_time': //
                'useraction':  // 用户处理情况
            }
            // ...
        ]
        "message": "详情获取成功!",
        "status": 200
    }
