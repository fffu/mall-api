# （设计师）提交方案: commitDraft

- 设计师提交设计方案
- 初稿仅上传设计说明，图片关联酷家乐信息表3d链接也在此表获取，终稿需要上传各房间图片以及对应房间说明，以及整个终稿设计说明；
- 设计师上传自己案例也是按照房间进行上传并进行说明，默认存在进度表的终稿，与案例表进行关联

## 参数

    {
        'id': // 订单ID type为3就是案例id
        'solution': [//方案图片与描述
            {
                'image_id': // 图片ID
                'explain': // 设计描述
            },
            // ...
        ],
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