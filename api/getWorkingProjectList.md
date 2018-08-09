# （平台/公司/设计师）获取在建工地列表: getWorkingProjectList

## 参数

    {
        'company_id': // 公司id，默认为空。
        'designer_id': // 设计师id，默认为空。
        'keyword': // 用户查询的关键字，默认为空。
        'process': // 默认全部 1:施工中；2：已竣工；
        'isrecommend': // 默认为空，获取全部；1为获取推荐的。
        'isindex': // 默认为空，获取全部。1为获取index的。
        'style': // 风格id。
        'unit': // 户型id。
        'page':
        'size':
    }

## 返回数据

    {
        'project_list': [
            {
                'project_id': 工地id
                'village': // 小区名称
                'costomer_name': // 业主姓名
                'designer': // 设计师
                'foreman': // 工长
                'supervisor': // 监理
                'area': // 面积
                'unit': // 户型
                'style': // 风格
                'cost': // 造价
                'complete_status': // 施工状态
                'current_step': // 当前施工进度（大阶段nodeid）
                'location': {
                    'province': // 省
                    'city': // 市
                    'region': // 区
                    'address': // 地址
                    'longitude': // 经度
                    'latitude': // 纬度
                }
                'fans_num': // 关注数
                'cover':{
                    'ori_path': // 原始图路径
                    'big_path': // 大图路径
                    'mid_path': // 中图路径
                    'sml_path': // 小图路径
                }
            }
            // ...
        ],
        'page_total': // 数据总条数
        "message": "列表获取成功!",
        "status": 200
    }
