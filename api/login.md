# 登录 login

- 注册（register）需要返回同样的数据，以便于自动登录
- 这个接口原来已经有了，需要新增字段

## 返回数据

- 添加字段：province、city、avatar、level、coin、integral、fans等
- 修改字段：roles。对象列表修改为单一对象。

        {
            "easemobId": "",
            "easemobPwd": "",
            "hasHouse": false,
            "head": null,
            "mobile": '',
            "name": "",
            'level': 1, // 用户等级，1，2，3，4，5，6
            "objectId": 1, // 用户id
            "passScore": 80,
            'province': '', // 省份
            'city': '', // 市
            'region': '', // 区
            "roleType": "",
            'avatar': '', // 头像路径 120px左右那个图
            "coin": int", // 益币数量
            "integral": int", // 积分
            "fans": int", // 粉丝数
            "roles": {
                "objectId": int, // 角色id
                "remark": "",
                "roleName": "",
                "roleSign": ""
            },
            "sex": null,
            "sign": "",
            "token": "",
            "username": "",
            "videoTime": ""
        }

## 说明

- 每天第一次登陆送积分，之后不送，连续7天登陆额外送积分（如此循环） 具体给多少通过平台后台配置
- 用户注册赠送用户积分,具体给多少通过平台后台配置