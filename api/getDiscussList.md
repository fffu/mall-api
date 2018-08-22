# 获取吐槽: getDiscussList

- 非业主的评论

## 参数

    {
        "id": // 公司id
        "query": // 1为工地，2为设计，3为案例，默认为全部
        "page": //页码
        "size": //每页数量
    }

## 返回数据

    {
        "discuss_list": [
            {
                "user": { // 评论人
                    "avatar": "", // 头像路径
                    "nick": ""// 昵称
                },
                "time": int, // 评论时间
                "content": "", // 评论内容
            },
            // ...
        ],
        "item_total": int, // 数据总条数
        "message": "数据获取成功!",
        "status": 200
    }
