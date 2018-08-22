# （任务大厅）获取订单详情: getTaskProfile

- 用户任务大厅选择单个订单了解详情

## 参数

    {
        'id': // 订单id
    }

## 返回数据

    {
        'content': [
            {
                'layout_pic': { // 户型图路径
                    'ori_path': //原图
                    'big_path': //大图
                    'mid_path': //中图
                    'sml_path': //
                },
                'id': //点单id
                'sn': // 订单编号
                'level': // 订单等级，1，2，3，4，5，6
                'budget': // 设计预算
                'unit': // 户型
                'area': // 面积
                'style': // 风格
                'house_status': // '旧房翻新'||'新房'
                'house_type': // '跃层'||'平层'||'别墅'
                'village': // 小区名
                'province': // 省份
                'city': // 市
                'region': // 区
                'release_time': // 审核通过时间
                'create_tiem': // 创建时间
                'end_time': // 订单到期时间
                'need_num': //允许最大抢单人数
                'designder_num': //目前抢单设计师人数
                'designer_list':[ // 已经抢单的设计师
                    {
                        'id': //设计师id
                        'name': //设计师名称
                        'avatar':{ // 头像
                            'ori_path': //原图
                            'big_path': //大图
                            'mid_path': //中图
                            'sml_path': //小图
                        },
                        'level': //设计师等级
                    },
                    // ...
                ],
                'user_habit':{} // 用户完善订单的内容
                'info': // 用户的补充说明
            },
            // ...
        ]
        "message": "详情获取成功!",
        "status": 200
    }