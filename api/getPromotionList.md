# 获取装修公司活动列表: getPromotionList

- 前端页面展示最新装修公司活动的推荐列表

## 参数

    {
        'company_id': // 装修公司id。
        'keyword': // 用户查询的关键字，默认为空。
        'mark': // 默认为空 ，显示位置。
        'isrecommend': // 默认为空，获取全部；1为获取推荐的。
        'valid': // 默认为空，获取全部。1为获取有效期内的，2为过期的。
        'ishot': // 默认为空，获取全部。1为获取hot的。
        'isindex': // 默认为空，获取全部。1为获取index的。（平台的字段）
        'page': // 页码
        'size': // 页长
    }

## 返回数据

    {
        'action_list': [
            {
                'id': // 活动id
                'title': // 活动标题
                'discription': // 活动描述
                'url': // 活动详情页
                'cover': { // 封面图
                    'ori_path': // 原始图路径
                    'big_path': // 大图路径
                    'mid_path': // 中图路径
                    'sml_path': // 小图路径
                }
            },
            // ...
        ],
        'page_total': // 总页数
        "message": "列表获取成功!",
        "status": 200
    }

## 说明

- 返回数据按level倒序排序