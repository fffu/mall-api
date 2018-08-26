# 获取装修平台或公司活动详情: getPromotionList


## 参数

    {
        'id': //活动id。
       }

## 返回数据

    {
        "promotion_detail": 
            {
                "id": "", // 活动id
                "title": "", // 活动标题
                "content": "", // 活动内容
                "href": "", // 活动详情页地址，数据表添加活动链接地址字段（针对平台活动使用）
                "view_num": int // 阅读量
                "create_time": int // 创建时间
            },,
        "message": "列表获取成功!",
        "status": 200
    }

