# (设计师)提交案例信息操作: createCase

## 参数

    {
        'title': //案例名称
        'style_id': //风格id
        'layout_id': //户型id
        'village': string //小区名称
        'address': string //小区地址
        'longitude': "", // 经度
        'latitude': "", // 纬度
        'area':  //面积
        'cost':  //案例造价
        'cover_id': //封面图id
        'house_type': int//房屋类型 别墅，平层等
        'type': int//装修类型 家装、工装、软装
        'boutique':int  //是否精品 1为精品   
    }  

## 返回数据

    {
        "message": "提交成功!",
        "status": 200
    }
