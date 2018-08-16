# 获取设计师详情: getDesignerDetail

## 参数

    {
        "id": // 设计师id
    }

## 返回数据

    {
        "content": {
            "id": // 设计师id
            "name": // 设计师名字
            "phone": // 设计师电话
            "level": // 设计师等级
            "location": {
                "province": // 省
                "city": // 市
                "region": // 区
            }
            "score": // 评分
            "case_num": // 案例数
            "fans_num": // 人气数
            "work_years": // 从业年限
            "education": // 学历
            "school": // 学校
            "field": // 专业
            "good_part": // 擅长空间
            "good_style_list":[ // 擅长风格
                // ...
            ],
            "company": // 所属公司
            "photo":{ // 设计师照片
                "ori_path": // 原始图路径
                "big_path": // 大图路径
                "mid_path": // 中图路径
                "sml_path": // 小图路径
            },
            "honor": String // 个人荣誉
        },
        "message": "数据获取成功!",
        "status": 200
    }
