# 登录 login

- 这个接口原来已经有了，roles这个字段会从[获取用户信息](./getUserInfo.md)获取，这里可以不用返回。

## 返回数据

- 添加字段：province、city、avatar、level等
- 修改字段：roles。对象列表修改为单一对象。

        {
            "easemobId": "",
            "easemobPwd": "",
            "hasHouse": false,
            "head": null,
            "mobile": '',
            "name": "",
            "objectId": 1, // 用户id
            "passScore": 80,
            'province': '', // 省份
            'city': '', // 市
            'region': '', // 区
            "roleType": "",
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