# 获取订单详情: getTaskProfile

- 订单详情页
- 08-22 增加返回字段step_title

## 参数

    {
        'id': // 订单id
    }

## 返回数据

    {
        'content': {
            "id": 1, // 订单id
            "sn": "", // 订单编号11为数字的字符串
            "level": 1, // 订单等级，1，2，3，4，5，6
            "free": true, // 免费订单，false为付费订单
            "budget": 1, // 设计预算
            "unit": "", // 户型 "n室n厅n厨n卫n阳台"
            "area": 1, // 面积
            "style": "", // 风格
            "house_status": "", // "旧房翻新"||"新房"
            "house_type": "", // "跃层"||"平层"||"别墅"
            "village": "", // 小区名
            "province": "", // 省份
            "city": "", // 市
            "region": "", // 区
            "release_time": int,// 审核通过时间
            "create_tiem": int,// 创建时间
            "remain_time": int,// 订单剩余时间戳
            "step_num": 1, // 当前步骤数
            "step_title": "", // 当前步骤标题
            "step_discript": "", // 当前步骤描述，需要判断用户
            "layout_pic": { // 户型图路径
                "ori_path": "", // 原
                "big_path": "", // 大
                "mid_path": "", // 中
                "sml_path": "", // 小
            },
            "max-need": int, // 最大抢单人数
            "designer": [ // 订单当前设计师们
                {
                    "name": "", // 名字
                    "objectId": int, // id
                    "avatar": "", // 头像路径 120px左右那个图
                    "level": 1, // 设计师等级，1，2，3，4，5，6
                }
            ]
        },
        "message": "详情获取成功!",
        "status": 200
    }