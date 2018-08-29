# （公司首页）查看公司设计师列表: getCompanyDesignerList

- 用户查看公司信息，只展示在职设计师

## 参数

    {
        'id': // 公司ID
        'keyword': // 用户查询的关键字，默认为空。
        'style': // 风格id，现代、田园 ...
        'sort_by': //排序按: 1人气，2评分，3案例数，4从业年限，5收费标准（字段不存在默认倒序，字段存在正序）
        'page': // 当前页
        'size': // 每页显示数量
    }

## 返回数据

    {
        'designer_list':[
            {
                'id': // 设计师id
                'name': // 设计师名字
                'level': // 设计师等级
                'title': // 设计师称谓；高级设计师、中级设计师、资深设计师...
                'location': {
                    'province': // 省
                    'city': // 市
                    'region': // 区
                }
                'work_years': // 从业年限
                'good_style': // 擅长风格
                'photo':{ // 设计师照片
                    'ori': // 原始图路径
                    'big': // 大图路径
                    'mid': // 中图路径
                    'sml': // 小图路径
                },
                'case_num': // 案例数
                'case_list': [ // 3条案例
                    {
                        'id': // 案例id
                        'name': // 案例名
                        'cover': { // 案例封面图
                            'ori': // 原始图路径
                            'big': // 大图路径
                            'mid': // 中图路径
                            'sml': // 小图路径
                        }
                    }
                    // ...
                ]
            },
            // ...
        ],
        "item_total": int, // 数据总条数
        "message": "数据获取成功!",
        "status": 200
    }
