# 所有个人用户提交认证操作: personageCertificate

- 包括设计师工长监理等角色认证也使用该接口， 选择角色后才能选择公司， 没选择公司就默认平台，普通用户不需要关联公司或平台

## 参数

    {
        'nick_name': //昵称
        'name': //用户真实姓名
        'sign': //用户个性标签
        'sex': //性别
        'province': // 省
        'city': // 市
        'region': // 区
        'address':// 详细地址
        'company_id': //公司id（认证设计师，工长，监理，材料经理，巡检等使用）（普通用户不用选，其余角色必须选公司，默认为益装网为第一个）
        'role_id': //角色id（下拉框，默认普通用户）
        'good_style': //擅长风格（多选）
        'good_port': //擅长空间（多选）
        'year': //从业年限
        'honor': string //荣誉
        'idea': //理念
        'charge': //收费标准（根据等级进行最低标准确认，不得低于这个标准）
        'description': //简介
        'school'://毕业学校
        'education'://学历
        'field': //专业
        'header_id'://头像id
        'qualification_id'://资质证书id
    }

## 返回数据

    {
        "message": "认证成功!",
        "status": 200
    }

## 说明

- 完成认证送积分 具体给多少通过平台后台配置
