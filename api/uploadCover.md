# （公司）上传活动封面图: uploadCover

## 参数

    {
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
