# （平台首页）获取公司列表：getCompanyList

## 参数

    {
        'query': {
            'keyword': // 用户查询的关键字，默认为空。
            'service_type': // 家装公司、工装公司、软装公司
            'region': // 区
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
                'id': // 公司ID
                'name': // 公司名
                'credit_level': // 信用级别
                'case_num': // 案例数
                'project_num': // 工地数
                'comment_num': // 公司评论数
                'location': {
                    'province': // 省
                    'city': // 市
                    'region': // 区
                    'address': // 地址
                    'longitude': // 经度
                    'latitude': // 纬度
                }
                'phone': // 公司电话
                'consult_num': // 公司咨询量
                'praise': // 口碑值
                'design_score': // 设计分
                'service_score': // 服务分
                'quality_score': // 工程质量分
                'project_score': // 工地分
                'logo': { // logo图
                    'ori_path': // 原始图路径
                    'big_path': // 大图路径
                    'mid_path': // 中图路径
                    'sml_path': // 小图路径
                }，
                'cover': { // 公司首页封面图
                    'ori_path': // 原始图路径
                    'big_path': // 大图路径
                    'mid_path': // 中图路径
                    'sml_path': // 小图路径
                }
            },
            // ...
        ],
        "item_total": int, // 数据总条数
        "message": "数据获取成功!",
        "status": 200
    }
