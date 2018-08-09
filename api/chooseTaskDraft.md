# （用  户）选择设计方案: chooseTaskDraft

- 用户在个人中心选择喜欢的方案（初稿、终稿）

## 参数

    {
        'id': Int, // 订单ID
        'process_id': Int, // 进度ID
        'isselected': Boolean // 选择||淘汰
        'explain': String // 理由
        'process_type': // 0：初稿；1：终稿；2：施工图
    }

## 返回数据

    {
        "message": "操作成功!",
        "status": 200
    }

## 说明

- 需要根据进度类型process_type判断该进度用户是否达到了选择案例数量上限，达到返回message错误提示
- 用户选择的设计稿给予设计师积分奖励，多少由后台配置
- 如果用户初稿，终稿选择个数够了，其余没有设计师的订单状态就全部改为完结，不能继续操作
