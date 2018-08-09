# （设计师，用户，公司公用）获取订单列表: getMyTaskList

- 个人中心，查看我的订单

## 参数

    {
        'page': //页码
        'size': //每页数量
        'status': // 空：全部；1：订单进行中；2：订单已完结；此状态需从设计师与订单关联表中查看
    }

## 返回数据

    {
       'tasklist': [ //array订单列表
            {
                'id': 1, // 订单id
                'sn': '', // 订单编号11为数字的字符串
                'level': 1, // 订单等级，1，2，3，4，5，6
                'free': true, // 免费订单，false为付费订单
                'budget': 1, // 设计预算
                'unit': '', // 户型 "n室n厅n厨n卫n阳台"
                'area': 1, // 面积
                'style': '', // 风格
                'house_status': '', // '旧房翻新'||'新房'
                'house_type': '', // '跃层'||'平层'||'别墅'
                'village': '', // 小区名
                'province': '', // 省份
                'city': '', // 市
                'region': '', // 区
                'release_time': int,// 审核通过时间
                'create_tiem': int,// 创建时间
                'remain_time': int,// 订单剩余时间戳
                'step_num': 1, // 当前步骤数
                'step_discript': '', // 当前步骤描述
                'layout_pic': { // 户型图路径
                    'ori_path': '', // 原
                    'big_path': '', // 大
                    'mid_path': '', // 中
                    'sml_path': '', // 小
                },
                "max-need": int, // 最大抢单人数
                'designer': [ // 订单当前设计师们
                    {
                        "name": "", // 名字
                        "objectId": int, // id
                        'avatar': '', // 头像路径 120px左右那个图
                        'level': 1, // 设计师等级，1，2，3，4，5，6
                    }
                ]
            }
        ]
        "page_total": int, //数据总条数
        "message": "列表获取成功",
        "status": 200
    }