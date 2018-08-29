# 公司提交认证操作: companyCertificate


## 参数

    {
        'nick_name': //昵称
        'name': //公司的全称
        'company_phone': //公司电话
        'province': // 省
        'city': // 市
        'region': // 区
        'address':// 详细地址
        'latitude':// 经度
        'longitude':// 维度
        'service_type': //公司服务类型：家装，工装，软装（多选）
        'good_style': //擅长风格（多选）
        'create_day': //成立日期
        'year': //成立年限
        'honor': string //荣誉
        'idea': //理念
        'legal_person'://法人
        'operation_period'://经营有效期
        'registered_capital': //注册资金
        'register_department': //登记机关
        'registered_address': //登记地址
        'inspection_time': //年检日期
        'introduction ':string //公司简介
        'introduction ':string //企业类型有限公司，集团公司等
        'header_id'://头像id
        'logo_id'://公司logo_id
        'qualification_id'://资质证书id
        'back_image'://公司首页背景图id
    }

## 返回数据

    {
        "message": "认证成功!",
        "status": 200
    }

## 说明

- 完成认证送积分 具体给多少通过平台后台配置
