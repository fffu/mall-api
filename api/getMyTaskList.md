# （设计师，用户，公司公用）获取我的订单列表: getMyTaskList

- 个人中心，查看我的订单
- 08-23 增加返回字段info，客户的备注信息
- 08-22 08-22 增加返回字段step_title，以及设计师的进度字段
- 08-21 修改查询字段及逻辑说明
- 08-09 getMyTaskList(获取我的订单)增加返回字段：max-need 最大抢单人数、designer[n].level 设计师的等级

## 参数

    {
        "user_id": int, // 用户或设计师的id，
        "page": //页码
        "size": //每页数量
        "status": // 空：全部；1：订单进行中；2：订单已完结；此状态需从设计师与订单关联表中查看
    }

- 登录用户与user_id匹配，或者为user_id的公司

## 返回数据

    {
       "tasklist": [ //array订单列表
            {
                "id": 1, // 订单id
                "sn": "", // 订单编号11为数字的字符串
                "level": 1, // 订单等级，1，2，3，4，5，6
                "free": true, // 免费订单，false为付费订单
                "budget": 1, // 设计预算
                "unit": "", // 户型 "n室n厅n厨n卫n阳台"
                "area": 1, // 面积
                "style": "", // 风格
                "house_status": "", // "旧房翻新"||"新房"
                "house_type": "", // "跃层"||"平层"||"别墅"
                "village": "", // 小区名
                "info": "", // 备注
                "province": "", // 省份
                "city": "", // 市
                "region": "", // 区
                "release_time": int,// 审核通过时间
                "create_tiem": int,// 创建时间
                "remain_time": int,// 订单剩余时间戳
                "step_id": 1, // 当前步骤id，订单表
                "step_title": "", // 当前步骤标题
                "step_discript": "", // 当前步骤描述
                "layout_pic": { // 户型图路径
                    "ori_path": "", // 原
                    "big_path": "", // 大
                    "mid_path": "", // 中
                    "sml_path": "", // 小
                },
                "max-need": int, // 最大抢单人数
                "designer": [ // 订单当前设计师们
                    {
                        "name": "", // 名字
                        "id": int, // 设计师id
                        "avatar": "", // 头像路径 120px左右那个图
                        "level": 1, // 设计师等级，1，2，3，4，5，6
                        "step_id": 1, // 当前步骤id，设计师与订单的关联表
                        "step_title": "", // 当前步骤标题
                        "step_discript": "", // 当前步骤描述
                    }
                ]
            }
        ]
        "item_total": int, // 数据总条数
        "message": "列表获取成功",
        "status": 200
    }

step相关的字段是**订单主表**的数据，designer下的step相关字段是**设计师与订单的关联表**的数据