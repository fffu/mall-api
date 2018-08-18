# 获取公司资料信息: getCompanyDetail

## 参数

    {
        'company_id': // 装修公司id
    }

## 返回数据

    {
        "intro": "", // 公司介绍，html字符串
        "registration": [ // 注册信息
            {
                "title": "", // 字段名，如：成立日期，注册资金等
                "txt": "" // 字段值，如：2013-10-18，为完善等
            }
            // ...
        ],
        "license": [ // 证书
            {
                "title": "@ctitle(3,13)", // 字段名，如：生产许可证、营业执照等
                "photo": { // 照片路径
                    "big": "", // 大图PC
                    "mid": "", // 中途wap
                }
            }
            // ...
        ],
        "message": "数据获取成功!",
        "status": 200
    }
