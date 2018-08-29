# (公司)提交活动操作: createPromotion

## 参数

    {
        'position_id': //展示位置id
        'ad_title': //广告名称
        'ad_content': //广告内容（富文本）
        'area_name': string //活动有效地区
        'start_time':  //活动开始时间
        'end_time':  //活动结束时间
        'is_show': //是否公司首页显示
        'is_hot': //是否热门
        'is_recommend': //是否推荐
        'cover_id': //封面图id
        'province_id': //所属省
        'city_id': //所属城市
        'region_id': //所属区
    }  

## 返回数据

    {
        "message": "提交成功!",
        "status": 200
    }
