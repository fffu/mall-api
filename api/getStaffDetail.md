# 获取员工详情: getStaffDetail

## 参数

    {
        "id": // 设计师id
    }

## 返回数据

    {
        "content": {
            "id": int, // 员工id
            "name": "", // 员工名字
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
            "case_num": int, // 案例数
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
