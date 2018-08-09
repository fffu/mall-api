# （设计师）获取订单进度详情: getDesignerTaskProcess

- 设计师查看自己单个订单的进度状态

## 参数

    {
        'id': // 订单ID
    }

## 返回数据

    {
        'content': {
            'my_step_list':[
                {
                    'process_id': // 进度ID
                    'stepnum':  // 进度步骤数
                    'steptitle':  // 进度步骤名称
                    'choose':  // 用户选择状态
                    'examine':  // 步骤审核状态 判断是否需要修改设计
                }
                // ...
            ],
            'order_status': //订单状态，从设计师与订单关联表查
        },
        "message": "列表进度成功!",
        "status": 200
    }