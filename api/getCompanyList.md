# （平台首页）获取公司列表：getCompanyList

## 参数

    {
        "location_id": int // 地区id
        'query': {
            'keyword': // 用户查询的关键字，默认为空。
            'service_type': // 家装公司、工装公司、软装公司
            'credit_level': // 信用等级
            'ensure': // 装修保障
            'isrecommend': // 默认空；1为推荐的公司
            'isindex': // 默认为空，获取全部。1为获取index的。
        },
        'sort': String, // total_score总评分\praise口碑\design设计分\service服务分\quality工程质量分\project_score工地分\（字段存在正序，不存在默认倒序）
        'page': // 页码
        'size': // 页长
    }

## 返回数据

    {
        'company_list': [
            {
                'id': int, // 公司ID
                'name': "", // 公司名
                "level": int, // 公司等级，1，2，3，4，5，6
                'design_case': int, // 设计案例数
                'project_case': int, // 施工案列数
                'aftermarket_case': int, // 售后案列数
                'credit_level': int, // 信用级别
                'location': {
                    'province': "", // 省
                    'city': "", // 市
                    'region': "", // 区
                    'address': "", // 地址
                    'longitude': "", // 经度
                    'latitude': "", // 纬度
                },
                'phone': "", // 公司电话
                'praise': int, // 口碑值
                "avatar": "", // 头像路径 120px左右那个图
            },
            // ...
        ],
        "item_total": int, // 数据总条数
        "message": "数据获取成功!",
        "status": 200
    }
