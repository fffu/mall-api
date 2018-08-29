# 获取装修公司活动列表: getPromotionList

- 前端页面展示最新装修公司活动的推荐列表
- 08-15 增加有效期"validity"、阅读量"view_num"

## 参数

    {
        'company_id': //默认空获取平台活动 ，公司id 存在获取装修活动。
        'keyword': // 用户查询的关键字，默认为空。
        'mark': // 默认为空 ，显示位置。
        'is_recommend': // 默认为空，获取全部；1为获取推荐的。
        'is_valid': // 默认为空，获取全部。1为获取有效期内的，2为过期的。
        'is_hot': // 默认为空，获取全部。1为获取hot的。
        'is_index': // 默认为空，获取全部。1为获取index的平台首页展示。（平台的字段）
        'show_company_index': // 默认为空，获取全部。1为获取index的首页展示。（公司的字段）
        'page': // 页码
        'size': // 页长
    }

## 返回数据

    {
        "promotion_list": [
            {
                "id": "", // 活动id
                "title": "", // 活动标题
                "discription": "", // 活动描述
                "href": "", // 活动详情页地址
                "cover": { // 封面图
                    "big": "", // 大图PC
                    "mid": "", // 中图wap
                },
                "validity": { // 有效期
                    "start": int, // 开始时间
                    "end": int, // 结束时间
                    "isValid": Boolen // 是否在有效期内
                }
                "view_num": int // 阅读量
                'show_time':int //显示时长
                'region':string //活动地区
            },
            // ...
        ],
        "item_total": int, // 数据总条数
        "message": "列表获取成功!",
        "status": 200
    }

## 说明

- 返回数据按level倒序排序