# 删除图片: deletePicture

- 用户上传图片时，撤回操作

## 参数

    {
        'img_id': Int // 图片ID
        'scene':int //1为户型图，2为设计稿，3设计师上传的案例，4头像，5营业执照，6封面图
    }

### 返回数据

    {
        "message": "删除图片成功",
        "status": 200
    }
