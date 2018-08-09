# 创建订单: createTask

- 用户提交设计需求

## 参数

    {
        'designerID' Int, // 设计师ID，如果有此项，表示预约特定设计师
        'area': Number, // 房屋面积
        'unit': String, // 户型
        'village': String, // 所属小区
        'province_id': Int, // 省份ID
        'city_id': Int, // 市ID
        'district_id': Int, // 区县ID
        'budget': Number, // 设计预算
        'image_id': Int, // 户型图ID
        'task_id': Int, // 订单ID
        'info': String // 用户附加输入的需求详情
        'house_status': // 房屋状态，'旧房翻新'||'新房'
        'house_type': // 房屋类型，'跃层'||'平层'||'别墅'
    }

## 返回数据

    {
        "message": "删除图片成功!",
        "status": 200
    }

## 说明

- 用户发布订单，后台管理员审核通过，给予用户积分和益币（两种奖励都有）
- 具体给多少通过平台后台配置