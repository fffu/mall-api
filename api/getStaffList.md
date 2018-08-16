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
        "staff_list|8": [
            {
                "id": int, // id
                "name": "", // 名字
                "role_id": int, // 角色id
                "role_name": "", // 角色名：首席设计师等，需要查积分表配置表
                "design_case": int, // 设计案例数量
                "project_case": int, // 工地案例数量
                "level": int, // 等级
                "work_years": int, // 从业年限
                "photo": "", // 照片路径，大图，800px左右那张图
                "avatar": "", // 头像路径 120px
                "recommend_case": [ // 推荐案例，每个设计师、工长等都有一组推荐案例，设计师则设计案列，工长则工地案例
                    {
                        "id": int, // 案例id
                        "name": ", // 案例name,也许是小区名
                        "style": "", // 风格
                        "unit": "", // 户型
                        "house_type": "", // "跃层"||"平层"||"别墅"
                        "area": int, // 面积
                        "cost": int, // 案例造价
                        "funs_num": int, // 赞数
                        "cover": { // 封面图
                            "big": "", // 大图PC
                            "mid": "", // 中途wap
                        }
                    }
                    // ... more item
                ]
            }
        ],
        "item_total": int, // 数据总条数
        "message": "数据获取成功!",
        "status": 200
    }
