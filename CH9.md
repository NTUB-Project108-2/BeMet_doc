# 第九章 程式

## 9-1 元件清單及其規格描述
一、 元件清單

(一)、 App端

表 9-1-1、App Project 元件清單
    
|資料夾名稱|:||
|---|---|---|
|編號|檔案名稱|功能|
    
(二)、 伺服器端

表 9-1-2 伺服器端 Project 元件清單
|資料夾名稱:|\bean||
|---|---|---|
|編號|檔案名稱|功能|
|2-1-1|ActivityDateBean.java|設定ActivityDate屬性，提供獲取屬性和設定屬性的方法|
|2-1-2|ActivityInviteBean.java|設定|ActivityInvite屬性，提供獲取屬性和設定屬性的方法|
|2-1-3|ActivityLabelBean.java|設定ActivityLabel屬性，提供獲取屬性和設定屬性的方法|
|2-1-4|ActivityRemindBean.java|設定ActivityRemind屬性，提供獲取屬性和設定屬性的方法|
|2-1-5|CodeTableBean.java|設定CodeTable屬性，提供獲取屬性和設定屬性的方法|
|2-1-6|FriendBean.java|設定Friend屬性，提供獲取屬性和設定屬性的方法|
|2-1-7|FriendCustomization.java|設定FriendCustomization屬性，提供獲取屬性和設定屬性的方法|
|2-1-8|FriendGroupBean.java|設定FriendGroup屬性，提供獲取屬性和設定屬性的方法|
|2-1-9|GroupsBean.java|設定Groups屬性，提供獲取屬性和設定屬性的方法|
|2-1-10|ProblemReportBean.java|設定ProblemReport屬性，提供獲取屬性和設定屬性的方法|
|2-1-11|TimelineBean.java|設定Timeline屬性，提供獲取屬性和設定屬性的方法|
|2-1-12|UserCustomizationBean.java|設定UserCustomization屬性，提供獲取屬性和設定屬性的方法|
|2-1-13|UserInformationBean.java|設定UserInformation屬性，提供獲取屬性和設定屬性的方法|
|資料夾名稱:|\config||
|編號|檔案名稱|功能|
|2-2-1|FCMInitializer.java|初始化FireBase Cloud Messaging設定|
|2-2-2|MvcConfig.java|專案設定檔|
|2-2-3|PersistenceConfig.java|資料庫連線設定檔|
|2-2-4|SecurityConfig.java|登入設定檔|
|資料夾名稱:|\controller||
|編號|檔案名稱|功能|
|2-3-1|ActivityDateController.java|控制處理前端/App請求|
|2-3-2|ActivityInviteController.java|控制處理前端/App請求|
|2-3-3|ActivityLabelController.java|控制處理前端/App請求|
|2-3-4|ActivityRemindController.java|控制處理前端/App請求|
|2-3-5|CodeTableController.java|控制處理前端/App請求|
|2-3-6|FriendController.java|控制處理前端/App請求|
|2-3-7|FriendCustomization.java|控制處理前端/App請求|
|2-3-8|FriendGroupController.java|控制處理前端/App請求|
|2-3-9|GroupsController.java|控制處理前端/App請求|
|2-3-10|ProblemReportController.java|控制處理前端/App請求|
|2-3-11|TimelineController.java|控制處理前端/App請求|
|2-3-12|UserCustomizationController.java|控制處理前端/App請求|
|2-3-13|UserInformationController.java|控制處理前端/App請求|
|資料夾名稱:|\converter||
|編號|檔案名稱|功能|
|2-4-1|LocalDateTimeConverter.java|日期轉換設定檔|
|資料夾名稱:|\dao||
|編號|檔案名稱|功能|
|2-5-1|ActivityDateDAO.java|查詢ActivityDate資料表介面|
|2-5-2|ActivityInviteDAO.java|查詢ActivityInvite資料表介面|
|2-5-3|ActivityLabelDAO.java|查詢ActivityLabel資料表介面|
|2-5-4|ActivityRemindDAO.java|查詢ActivityRemind資料表介面|
|2-5-5|CodeTableDAO.java|查詢CodeTable資料表介面|
|2-5-6|FriendDAO.java|查詢Friend資料表介面|
|2-5-7|FriendCustomization.java|查詢FriendCustomization資料表介面|
|2-5-8|FriendGroupDAO.java|查詢FriendGroup資料表介面|
|2-5-9|GroupsDAO.java|查詢Groups資料表介面|
|2-5-10|ProblemReportDAO.java|查詢ProblemReport資料表介面|
|2-5-11|TimelineDAO.java|查詢Timeline資料表介面|
|2-5-12|UserCustomizationDAO.java|查詢UserCustomization資料表介面|
|2-5-13|UserInformationDAO.java|查詢UserInformation資料表介面|
|2-5-14|BaseDAO.java|資料庫基本操作功能介面|
|資料夾名稱:|\dao\impl||
|編號|檔案名稱|功能|
|2-6-1|ActivityDateDAO.java|查詢ActivityDate資料表實作|
|2-6-2|ActivityInviteDAO.java|查詢ActivityInvite資料表實作|
|2-6-3|ActivityLabelDAO.java|查詢ActivityLabel資料表實作|
|2-6-4|ActivityRemindDAO.java|查詢ActivityRemind資料表實作|
|2-6-5|CodeTableDAO.java|查詢CodeTable資料表實作|
|2-6-6|FriendDAO.java|查詢Friend資料表實作|
|2-6-7|FriendCustomization.java|查詢FriendCustomization資料表實作|
|2-6-8|FriendGroupDAO.java|查詢FriendGroup資料表實作|
|2-6-9|GroupsDAO.java|查詢Groups資料表實作|
|2-6-10|ProblemReportDAO.java|查詢ProblemReport資料表實作|
|2-6-11|TimelineDAO.java|查詢Timeline資料表實作|
|2-6-12|UserCustomizationDAO.java|查詢UserCustomization資料表實作|
|2-6-13|UserInformationDAO.java|查詢UserInformation資料表實作|
|2-6-14|BaseDAOImpl.java|資料庫基本操作功能實作|
|資料夾名稱:|\filter||
|編號|檔案名稱|功能|
|2-7-1|CustomAuthenticationFailureHandler.java|登入失敗回傳資料設定|
|2-7-2|CustomAuthenticationProvider.java|登入邏輯|
|2-7-3|CustomAuthenticationSuccessHalder.java|登入成功回傳資料設定|
|2-7-4|CustomAuthenticationToken.java|保存請求參數|
|2-7-5|CustomEntryPoint.java|未登入處理設定|
|2-7-6|CustomerAccessDeniedHalder.java|權限不足回傳資料設定|
|2-7-7|CustomLoginFilter.java|登入驗證|
|2-7-8|WebInterceptor.java|攔截用戶請求並進行處理|
|資料夾名稱:|\service||
|編號|檔案名稱|功能|
|2-8-1|ActivityDateService.java|ActivityDate相關業務邏輯介面|
|2-8-2|ActivityInviteService.java|ActivityInvite相關業務邏輯介面|
|2-8-3|ActivityLabelService.java|ActivityLabel相關業務邏輯介面|
|2-8-4|ActivityRemindService.java|ActivityRemind相關業務邏輯介面|
|2-8-5|CodeTableService.java|CodeTable相關業務邏輯介面|
|2-8-6|FriendService.java|Friend相關業務邏輯介面|
|2-8-7|FriendCustomizationService.java|FriendCustomization相關業務邏輯介面|
|2-8-8|FriendGroupService.java|FriendGroup相關業務邏輯介面|
|2-8-9|GroupsService.java|Groups相關業務邏輯介面|
|2-8-10|ProblemReportService.java|ProblemReport相關業務邏輯介面|
|2-8-11|TimelineService.java|Timeline相關業務邏輯介面|
|2-8-12|UserCustomizationService.java|UserCustomization相關業務邏輯介面|
|2-8-13|UserInformationService.java|UserInformation相關業務邏輯介面|
|資料夾名稱:|\service\impl||
|編號|檔案名稱|功能|
|2-9-1|ActivityDateServiceImpl.java|ActivityDate相關業務邏輯實作|
|2-9-2|ActivityInviteServiceImpl.java|ActivityInvite相關業務邏輯實作|
|2-9-3|ActivityLabelServiceImpl.java|ActivityLabel相關業務邏輯實作|
|2-9-4|ActivityRemindServiceImpl.java|ActivityRemind相關業務邏輯實作|
|2-9-5|CodeTableServiceImpl.java|CodeTable相關業務邏輯實作|
|2-9-6|FriendServiceImpl.java|Friend相關業務邏輯實作|
|2-9-7|FriendCustomizationServiceImpl.java|FriendCustomization相關業務邏輯實作|
|2-9-8|FriendGroupServiceImpl.java|FriendGroup相關業務邏輯實作|
|2-9-9|GroupsServiceImpl.java|Groups相關業務邏輯實作|
|2-9-10|ProblemReportServiceImpl.java|ProblemReport相關業務邏輯實作|
|2-9-11|TimelineServiceImpl.java|Timeline相關業務邏輯實作|
|2-9-12|UserCustomizationServiceImpl.java|UserCustomization相關業務邏輯實作|
|2-9-13|UserInformationServiceImpl.java|UserInformation相關業務邏輯實作|
|資料夾名稱:|\utils||
|編號|檔案名稱|功能|
|2-10-1|BCryUtility.java|密碼加密、密碼比對|
|2-10-2|BeanUtility.java|更新傳入物件的屬性值|
|2-10-3|ResponseUtils.java|請求回應設定|
|資料夾名稱:|\vo||
|編號|檔案名稱|功能|
|2-11-1|ActivityDate.java|資料庫ActivityDate資料表對映|
|2-11-2|ActivityInvite.java|資料庫ActivityInvite資料表對映|
|2-11-3|ActivityLabel.java|資料庫ActivityLabel資料表對映|
|2-11-4|ActivityRemind.java|資料庫ActivityRemind資料表對映|
|2-11-5|CodeTable.java|資料庫CodeTable資料表對映|
|2-11-6|Friend.java|資料庫Friend資料表對映|
|2-11-7|FriendCustomization.java|資料庫FriendCustomization資料表對映|
|2-11-8|FriendGroup.java|資料庫FriendGroup資料表對映|
|2-11-9|Groups.java|資料庫Groups資料表對映|
|2-11-10|ProblemReport.java|資料庫ProblemReport資料表對映|
|2-11-11|Timeline.java|資料庫Timeline資料表對映|
|2-11-12|UserCustomization.java|資料庫UserCustomization資料表對映|
|2-11-13|UserInformation.java|資料庫UserInformation資料表對映|
(三)、 網頁端
|資料夾名稱:|\templates||
|---|---|---|
|3-1-1|login.html|登入頁面|
|3-1-2|logout.html|登出頁面|
|資料夾名稱:|\templates\problem_report||
|---|---|---|
|3-2-1|add.html|問題回報頁面|
|3-3-2|index.html|問題回報管理者頁面|
|3-3-3|update.html|問題處理狀態修改頁面|
二、規格描述
(一)、 App端
(二)、 伺服器端
|編號|2-1|程式名稱||
|---|---|---|---|
|目的|
||
(二)、 網頁端