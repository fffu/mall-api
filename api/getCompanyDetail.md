# （公司首页）获取装修公司详情: getCompanyDetail

## 参数

    {
        'company_id': // 装修公司id
    }

## 返回数据

    {
        'content': {
            'id': // 装修公司id
            'name': // 装修公司名字
            'phone': // 电话
            'credit_level': // 装修公司信用等级
            'total_score': // 总评分
            'praise': // 装修公司口碑
            'design': // 装修公司设计分
            'service': // 装修公司服务分
            'quality': // 装修公司工程质量分
            'project': // 装修公司工地分
            'back_image': // 装修公司背景图路径
            'logo': { // logo图
                'ori_path': // 原始图路径
                'big_path': // 大图路径
                'mid_path': // 中图路径
                'sml_path': // 小图路径
            },
            'location': {
                'province': // 省
                'city': // 市
                'region': // 区
                'address': // 地址
            },
            'case_num': // 案例数
            'fans_num': // 人气数
            'introduce': // 公司简介
            'license': [ // 资质证书
                {
                    'ori_path': // 原始图路径
                    'big_path': // 大图路径
                    'mid_path': // 中图路径
                    'sml_path': // 小图路径
                }
                // ...
            ],
            'service_content': {//服务
                'type_list': Array, // id=>名称
                'region_list': Array, // id=>名称
                'price': String,
                'style': Array, // id=>名称
            }
        },
        "message": "数据获取成功!",
        "status": 200
    }
