# 所有用户提交认证操作: certificate

## 参数

    {
        'nick_name': //昵称
        'name': //用户真实姓名或者公司的全称
        'sex': //性别
        'province': // 省
        'city': // 市
        'region': // 区
        'address':// 详细地址
        'company_id': //公司id（认证设计师，工长，监理，材料经理，巡检等使用）（普通用户公司选项禁用默认益装网，其余角色必须选公司）
        'type': //1个人认证，2公司认证(单选)
        'role_id': //角色id（下拉框，默认普通用户）
        'service_type': //公司服务类型：家装，工装，软装（多选）
        'service_region': //服务区域（多选）
        'good_style': //擅长风格（多选）
        'good_port': //擅长空间（多选）
        'year': //从业经验
        'honor': string //荣誉
        'idea': //理念
        'school'://毕业学校
        'education'://学历
        'field': //专业
        'introduction ':string //公司简介
        'header_id'://头像id
        'logo_id'://公司logo_id
        'qualification_id'://资质证书id
    }

## 返回数据

    {
        "message": "认证成功!",
        "status": 200
    }

## 说明

- 完成认证送积分 具体给多少通过平台后台配置
