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
        "designer_list|8": [
            {
                "id": int, // 设计师id
                "name": "", // 设计师名字
                "level": int, // 设计师等级
                "work_years": int, // 从业年限
                "concept": "", // 设计师理念
                "photo": "", // 照片路径，大图，800px左右那张图
                "avatar": "", // 头像路径
                "case_num": int,// 案例数
            },
            // ...
        ],
        "item_total": int, // 数据总条数
        "message": "数据获取成功!",
        "status": 200
    }
