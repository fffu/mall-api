# （平台首页）推荐设计师列表: getIndexDesignerList

## 参数

    {
        'isrecommend': // 默认为空，获取全部；1为获取推荐的。
        'isindex': // 默认为空，获取全部。1为获取index的。
        'page': // 页码
        'size': // 页长
    }

## 返回数据

    {
        'designer_list': [
            {
                'id': // 设计师id
                'name': // 设计师名字
                'level': // 设计师等级
                'concept': // 设计师理念
                'photo': { // 照片
                    'ori_path': // 原始图路径
                    'big_path': // 大图路径
                    'mid_path': // 中图路径
                    'sml_path': // 小图路径
                }
                'case_num': // 案例数
            },
            // ...
        ],
        'page_total': // 总页数
        "message": "数据获取成功!",
        "status": 200
    }
