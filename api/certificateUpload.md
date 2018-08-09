# 认证专用上传图片: certificateUpload

- 用户上传头像，公司上传logo，公司设计师工长等上传从业资质证书公用接口，公司上传自己首页封面图，上传充值凭证

## 参数

    {
        'scene': Int, // 图片场景；0：用户上传头像；1：公司上传logo；2：公司设计师工长等上传从业资质证书；3公司上传自己首页封面图；4上传充值凭证
        'iamge_type': String, // 'image'
        'width': Int, // 图片宽度 px
        'height': Int, // 图片高度 px
        'size': Int, // 图片大小 bye
    }

## 返回数据

    {
        'content': {
            'img_id': Int // 图片ID
            'ori_path': // 原始图路径
            'big_path': // 大图路径
            'mid_path': // 中图路径
            'sml_path': // 小图路径
        },
        "message": "上传成功!",
        "status": 200
    }

## 说明

每次调用接口，仅上传一张图片,关联用户