# 益装网api需求

updates at the bottom, 更新日志在后面  
**避免浪费效率，建议先实现更新过的文档，没更新过的文档大都不完整或有缺陷**

## 目录

- [登录/注册](./api/login.md): login,register
- [上传图片](./api/uploadPicture.md): uploadPicture
- [删除图片](./api/deletePicture.md): deletePicture
- [创建订单](./api/createTask.md): createTask
- [用户完善订单信息(未定)](./api/improveTask.md): improveTask
- [(任务大厅)获取订单列表](./api/getTaskList.md): getTaskList
- [(任务大厅)获取订单详情](./api/getTaskDetail.md): getTaskDetail
- [(设计师/用户/公司公用)获取我的订单列表](./api/getMyTaskList.md): getMyTaskList, 和上面这个接口返回同样数据，能合并就合并
- [(设计师)抢单](./api/grabTask.md): grabTask
- [提交方案](./api/commitDraft.md): commitDraft
- [(设计师)获取订单进度详情](./api/getDesignerTaskProcess.md): getDesignerTaskProcess
- [(设计师)获取订单设计详情](./api/getDesignerTaskDraft.md): getDesignerTaskDraft
- [(用户)获取订单设计详情](./api/getTaskDraft.md): getTaskDraft
- [(用户)选择设计方案](./api/chooseTaskDraft.md): chooseTaskDraft
- [(用户)评价](./api/commentTask.md): commentTask
- [(公司)查看订单详情](./api/getCompanyTaskDetail.md): getCompanyTaskDetail
- [(公司)审核设计师的设计](./api/reviewDraft.md): reviewDraft
- [(公司)查看员工列表](./api/getStaffList.md): getStaffList
- [(公司)员工操作](./api/manageStaff.md): manageStaff
- [(公司)查看工地列表](./api/getCompanyProjectList.md): getCompanyProjectList
- [获取公司列表](./api/getCompanyList.md): getCompanyList
- [获取公司简要信息](./api/getCompanyProfile.md): getCompanyProfile，上面接口的单个版
- [查看公司设计师列表](./api/getCompanyDesignerList.md): getCompanyDesignerList
- [获取装修公司活动列表](./api/getPromotionList.md): getPromotionList
- [获取在建工地列表](./api/getWorkingProjectList.md): getWorkingProjectList
- [喜欢点赞](./api/like.md): like
- [(平台首页)推荐设计师列表](./api/getIndexDesignerList.md): getIndexDesignerList
- [(平台/公司/设计师)获取案例列表](./api/getCaseList.md): getCaseList
- [获取装修公司详情](./api/getCompanyDetail.md): getCompanyDetail
- [获取设计师详情](./api/getDesignerDetail.md): getDesignerDetail
- [获取公司评价](./api/getCommentList.md): getCommentList
- [非业主评论(工地、设计、案例)](./api/discuss.md): discuss
- [所有用户提交认证操作](./api/certificate.md): certificate
- [认证专用上传图片](./api/certificateUpload.md): certificateUpload
- [充值](./api/recharge.md): recharge
- [公司名模糊查询](./api/getCompanyName.md): getCompanyName
- [设计师发起公司变更操作](./api/changeMyCompany.md): changeMyCompany
- [(公司)提交活动操作](./api/createPromotion.md): createPromotion
- [(公司)上传活动封面图](./api/uploadCover.md): uploadCover
- [获取用户信息](./api/getUserInfo.md): getUserInfo

## 保持更新，请注意变更情况

- 0812 新增[获取公司简要信息](./api/getCompanyProfile.md): getCompanyProfile，[获取公司列表](./getCompanyList.md) 的单个版
- 0812 修改[获取公司列表](./api/getCompanyList.md)
- 0811 修改[获取公司列表](./api/getCompanyList.md)
- 0811 修改[登录/注册](./api/login.md)的说明
- 0810 [(平台首页)推荐设计师列表](./api/getIndexDesignerList.md) 更改返回数据模板
- 0810 所有接口的 数据总条数 健 "page_total" 改为 "item_total"
- 0810 修改[获取装修公司活动列表](./api/getPromotionList.md)返回数据模板
- 0809 getMyTaskList(获取我的订单)增加返回字段：

  - max-need 最大抢单人数
  - designer[n].level 设计师的等级
  - getTaskList(任务大厅拉取订单列表)更改为返回getMyTaskList(获取我的订单)一样的数据

- 0808更新：

  - 合并了设计师、用户、公司获取'我的列表'三个接口为一个接口：getMyTaskList，并完善了该接口
  - 修改了注册登录接口的字段

- 0807 更改注册接口需要返回登录的数据，以便于自动登录：
- 0728am更新：

  - 添加了各个接口的名称，[前端的模拟请求](./src/mock.js)使用了这些名称。路径待定。
  - 删除了两个讨论之后废弃/合并的接口