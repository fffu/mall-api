# （公  司）查看员工列表: getStaffList

## 参数

    {
        'type': // 默认为空查询在职
        'role_id': // 角色id；默认为3；设计师3，工长11，工程部经理12，材料部经理13，监理14，巡检15
        'page': // 当前页
        'size': // 每页显示数量
    }

## 返回数据

    {
        'staff_list':[
            {
                'name': // 设计师名字
                'id': // 设计师id
                'level': // 设计师等级
                'title': // 设计师称谓；高级设计师、中级设计师、资深设计师...
                'isincumbent': 1||2 // 1:入职；2：在职；3.离职。
                'location': {
                    'province': // 省
                    'city': // 市
                    'region': // 区
                }
                'work_years': // 从业年限
                'good_style': // 擅长风格
                'photo':{
                    'ori_path': // 原始图路径
                    'big_path': // 大图路径
                    'mid_path': // 中图路径
                    'sml_path': // 小图路径
                }
            },
            // ...
        ],
        "item_total": "@natural(20,999)", // 数据总条数
        "message": "数据获取成功!",
        "status": 200
    }
