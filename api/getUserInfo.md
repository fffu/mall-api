# 获取用户信息: getUserInfo

## 参数

    {
        "id": int, // 用户id
    }

## 返回数据

    {
        "info": {
            "name": "", // 用户名
            "role": {
                "id": int, // 角色id
                "remark": "",
                "name": "", // 角色名，需要查角色的积分配置表
                "roleSign": ""
            },
            "level": int, // 用户等级，1，2，3，4，5，6
            "avatar": "", // 头像路径 120px左右那个图
            "coin": int, // 益币数量
            "integral": int, // 积分
            "fans": int, // 粉丝数
            "new_msn": int, // 新消息数目
            "new_task": int, // 新订单数目
        },
        "message": "获取数据成功!",
        "status": 200
    }

## 说明

- 此时不要更新消息已读状态
- 此时不要更新订单的查看状态