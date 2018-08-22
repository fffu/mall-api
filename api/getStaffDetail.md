# 获取员工详情: getStaffDetail

- 设计师，工长等详情页展示

## 参数

    {
        "id": // 设计师id或工长等id
    }

## 返回数据

    {
        "content": {
            "id": int, // 员工id
            "name": "", // 员工名字
            "role_id": int, // 角色id
            "role_name": "", // 角色名：首席设计师等，需要查积分表配置表
            "phone": "", // 员工电话
            "level": int, // 员工等级
            "location": {
                "province": "", // 省
                "city": "", // 市
                "region": "", // 区
                "address": "", // 地址
                "longitude": "", // 经度
                "latitude": "", // 纬度
            },
            "score": float, // 评分
            "design_case": int, // 设计案例数
            "project_case": int, // 施工案列数
            "fans_num": int, // 人气数
            "work_years": int, // 从业年限
            "education": "", // 学历
            "school": "", // 学校
            "field": "", // 专业
            "good_part": [ // 擅长空间
                {
                    "id": int, // 空间id
                    "txt": "" // 空间名
                }
            ],
            "good_style": [ // 擅长风格
                {
                    "id": int, // 风格id
                    "txt": "" // 风格名
                }
            ],
            "company": "", // 所属公司
            "avatar": "", // 头像路径
            "honor": [ // 个人荣誉
                "",
                // ...
            ],
        },
        "message": "数据获取成功!",
        "status": 200
    }
