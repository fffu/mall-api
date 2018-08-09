# （公  司）查看订单详情: getCompanyTaskDetail

- 公司个人中心查看订单详情和设计师提交的方案

## 参数

    {
        'id': // 订单id
        'designer_id': // 设计师id
    }

## 返回数据

    {
        'content': {
            'content': [
                {
                    'task': {
                        'sn': // 订单编号
                        'release_time': // 订单发布时间
                        'area': // 面积
                        'unit': // 户型
                        'house_status': // '旧房翻新'||'新房'
                        'house_type': // '跃层'||'平层'||'别墅'
                        'province': // 省
                        'city': // 市
                        'region': // 区
                        'village': // 小区名称
                        'design_budget': // 设计预算
                        'budget': // 装修预算
                        'info': // 备注内容
                        'address': // 地址
                        'measure_time': // 量房时间
                        'customer': {
                            'name': // 客户姓名
                            'hobby': // 爱好
                            'phone': // 客户电话，此字段需鉴权，用户选择初稿后才返回此字段
                            'members': [
                                {
                                    'relation': // 与用户的关系，父亲、母亲..
                                    'age': // 年龄
                                    'hobby': // 爱好
                                    'style': // 偏爱风格
                                    'color': // 偏好颜色
                                    'info': // 备注
                                }
                                // ...
                            ]
                        },
                        'step_title': // 进度状态，从进度表查询
                    },
                    'solution': { // 方案
                        'designer_id': // 设计师id
                        'designer_name': // 设计师姓名
                        'first_draft': { // 初稿
                            'process_id': // 进度id
                            '3d_url': //3d
                            'examine_time': // 审核时间
                            'content': [
                                {
                                    'image':{
                                        'small_path': String, // 图片路径
                                        'medium_path': String, // 图片路径
                                        'big_path': String, // 图片路径
                                    }
                                    'part_name': // 房间名称
                                    'explain': // 设计描述
                                },
                                // ...
                            ],
                            'explain': //
                            'useraction':  // 用户处理情况
                        },
                        'final_draft':{ // 终稿
                            'process_id': // 进度id
                            '3d_url': //3d链接
                            'examine_time': //审核时间
                            'content': [
                                {
                                    'image':{
                                        'small_path': String, // 图片路径
                                        'medium_path': String, // 图片路径
                                        'big_path': String, // 图片路径
                                    }
                                    'part_name': // 房间名称
                                    'explain': // 设计描述
                                },
                                // ...
                            ],
                            'explain': //
                            'useraction':  // 用户处理情况
                        },
                        'cad':{ // 施工图凭证
                            'process_id': //进度id
                            'examine_time': //审核时间
                            'image':{
                                'small_path': String, // 图片路径
                                'medium_path': String, // 图片路径
                                'big_path': String, // 图片路径
                            }
                            'explain': // 施工图凭证描述
                        },
                    }
                }
                // ...
            ]
        },
        "message": "详情获取成功!",
        "status": 200
    }