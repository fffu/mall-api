# (公司)提交活动操作: createPromotion

## 参数

    {
        'position_id': //展示位置id
        'ad_title': //广告名称
        'ad_content': //广告内容
        'ad_link': //广告链接
        'area_name': string //活动有效地区
        'start_time':  //活动开始时间
        'end_time':  //活动结束时间
        'link_type': int //活动内链或外链 0-外部链接 1-内容链
        'link_type': int //活动内链或外链 0-外部链接 1-内容链
        'is_show': //是否公司首页显示
        'is_hot': //是否热门
        'is_recommend': //是否推荐
        'cover_id': //封面图id
        'province_id': //所属省
        'city_id': //所属城市
        'region_id': //所属区
        'type':int //该活动属于公司1为平台，2为公司
    }  

## 返回数据

    {
        "message": "提交成功!",
        "status": 200
    }
