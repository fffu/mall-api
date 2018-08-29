# 员工离职或申请加入公司申请：auditLaborTurnover

- 用于公司审核员工离职或加入申请操作，审核通过恢复员工与平台关联数据

## 参数

    {
        'user_id':  //员工id
        'choose': int //审核状态1通过或者0不通过
        'type':int //1为离职申请，2为加入申请
    }
    
## 返回参数

    {
        "message": "操作成功!",
         "status": 200
    }

