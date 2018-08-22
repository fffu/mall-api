# 益装网api需求

目录条目前的数字表示最后更改的日期，若无，表示至初稿后还未更新  
**避免浪费效率，建议先实现更新过的文档，没更新过的文档大都不完整或有缺陷**

## 页面展示类

- 08-11 [登录/注册](./api/login.md): login,register

- 获取获取订单信息

  - 08-22 [(任务大厅)获取订单列表](./api/getTaskList.md): getTaskList
  - 08-22 [获取我的订单列表](./api/getMyTaskList.md): getMyTaskList
  - 08-22 [获取订单详情](./api/getTaskProfile.md): getTaskProfile  
    <small>以上三个返回了同样的数据模板，不同的是返回 **多条** 或 **一条**</small>
  <!-- - [(设计师)获取订单进度详情](./api/getDesignerTaskProcess.md): getDesignerTaskProcess -->
  - [(设计师)获取订单设计详情](./api/getDesignerTaskDraft.md): getDesignerTaskDraft
  <!-- - [(用户)获取订单设计详情](./api/getTaskDraft.md): getTaskDraft -->
  <!-- - [(公司)查看订单详情](./api/getCompanyTaskDetail.md): getCompanyTaskDetail -->

- 获取用户信息相关

  - 08-12 [获取公司列表](./api/getCompanyList.md): getCompanyList
  - 08-12 [获取公司简要信息](./api/getCompanyProfile.md): getCompanyProfile，上面接口的单个版
  - 08-18 [获取公司资料信息](./api/getCompanyDetail.md): getCompanyDetail
  - [公司名模糊查询](./api/getCompanyName.md): getCompanyName
  - 08-16 [查看员工列表](./api/getStaffList.md): getStaffList
  - 08-10 [首页推荐设计师列表](./api/getIndexDesignerList.md): getIndexDesignerList
  - 08-17 [获取员工详情](./api/getStaffDetail.md): getStaffDetail
  - 08-18 [获取用户信息](./api/getUserInfo.md): getUserInfo
  - 08-17 [获取案例列表](./api/getCaseList.md): getCaseList
  - 08-16 [获取案例详情](./api/getCaseDetail.md): getCaseDetail
  - [查看工地列表](./api/getCompanyProjectList.md): getCompanyProjectList
  - 08-16 [获取在建工地列表](./api/getWorkingProjectList.md): getWorkingProjectList
  - 08-15 [获取装修公司活动列表](./api/getPromotionList.md): getPromotionList

## 数据操作类

- 通用操作

  - [上传图片](./api/uploadPicture.md): uploadPicture
  - [删除图片](./api/deletePicture.md): deletePicture
  - [喜欢点赞](./api/like.md): like
  - [吐槽](./api/discuss.md): discuss
  - [获取吐槽](./api/getDiscussList.md): getDiscussList
  - [所有用户提交认证操作](./api/certificate.md): certificate
  - [认证专用上传图片](./api/certificateUpload.md): certificateUpload
  - [充值](./api/recharge.md): recharge

- 订单操作相关

  - [创建订单](./api/createTask.md): createTask
  - [用户完善订单信息(未定)](./api/improveTask.md): improveTask
  - [(设计师)抢单](./api/grabTask.md): grabTask
  - [提交方案](./api/commitDraft.md): commitDraft
  - [(用户)选择设计方案](./api/chooseTaskDraft.md): chooseTaskDraft
  - [(用户)评价](./api/commentTask.md): commentTask
  - [(公司)审核设计师的设计](./api/reviewDraft.md): reviewDraft

- 公司管理操作

  - [公司管理员工状态](./api/manageStaff.md): manageStaff
  - [员工离职申请](./api/laborTurnover.md): laborTurnover
  - [公司审核员工离职申请](./api/auditLaborTurnover.md): auditLaborTurnover
  - [设计师发起公司变更操作](./api/changeMyCompany.md): changeMyCompany
  - [公司提交活动操作](./api/createPromotion.md): createPromotion
  - [(公司)上传活动封面图](./api/uploadCover.md): uploadCover