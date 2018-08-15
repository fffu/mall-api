# 获取装修公司活动列表: getPromotionList

- 前端页面展示最新装修公司活动的推荐列表

## 参数

    {
        'company_id': // 装修公司id。
        'keyword': // 用户查询的关键字，默认为空。
        'mark': // 默认为空 ，显示位置。
        'isrecommend': // 默认为空，获取全部；1为获取推荐的。
        'isvalid': // 默认为空，获取全部。1为获取有效期内的，2为过期的。
        'ishot': // 默认为空，获取全部。1为获取hot的。
        'isindex': // 默认为空，获取全部。1为获取index的。（平台的字段）
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
                "cover": "", // 封面图路径
                "validity": { // 有效期
                    "start": int, // 开始时间
                    "end": int, // 结束时间
                    "isValid": Boolen // 是否在有效期内
                }
                "view_num": int // 阅读量
            },
            // ...
        ],
        "item_total": int, // 数据总条数
        "message": "列表获取成功!",
        "status": 200
    }

## 说明

- 返回数据按level倒序排序