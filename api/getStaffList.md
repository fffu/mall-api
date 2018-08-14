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
        "stuff_list|8": [
            {
                "id": int, // id
                "name": "", // 名字
                "role_id": int, // 角色id
                "level": int, // 等级
                "work_years": int, // 从业年限
                "photo": "", // 照片路径，大图，800px左右那张图
                "avatar": "", // 头像路径 120px
            }
        ],
        "item_total": int, // 数据总条数
        "message": "数据获取成功!",
        "status": 200
    }
