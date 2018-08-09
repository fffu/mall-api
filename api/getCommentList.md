# （公司页面）获取公司评价: getCommentList

## 参数

    {
        'id': // 公司id
        'query': // 1为工地，2为设计，3为案例，默认为1
    }

## 返回数据

    {
        'comment_list': [
            {
                'user': { // 评论人
                    'avatar': { // 头像
                        'ori_path': // 原始图路径
                        'big_path': // 大图路径
                        'mid_path': // 中图路径
                        'sml_path': // 小图路径
                    },
                    'nick': // 昵称
                },
                'time': // 评论时间
                'content': // 评论内容
            },
            // ...
        ],
        "message": "数据获取成功!",
        "status": 200
    }
