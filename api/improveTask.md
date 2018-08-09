# 用户完善订单信息（未定）

- 客户创建订单（任务）后，填写的个人生活习惯等信息，提供给设计师

## 参数

    {
        'members': [  // 家庭成员 Array
            {
                'name': String, // 名字
                'age': Int, // 年龄
                'style': String, // 倾向风格
                'interest': String, // 爱好
                'color': String, // 偏爱颜色
                'info': String, // 备注
            },
            // ……
        ],
        'coustoms': {
            'intercourse': ''
        }
    }

## 返回数据

    {
        "message": "提交信息成功",
        "status": 200
    }

## 说明

- 完善订单补充信息送积分 具体给多少通过平台后台配置