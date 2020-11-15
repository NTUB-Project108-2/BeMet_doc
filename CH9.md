# 第九章 程式

## 9-1 軟體架構與程式清單
一、 軟體架構
![](https://i.imgur.com/r5KDc56.jpg)
![](https://i.imgur.com/5lZQ9VA.jpg)
二、 程式清單
(一)、 App端

表 9-1-1、App Project 元件清單
    
|資料夾名稱:\adapter|||
|---|---|---|
|編號|檔案名稱|功能|
|1-1-1|EventAddParticipantRecyclerViewAdapter.java|設定事件參與者recycler view 畫面|
|1-1-2|EventTagRecyclerViewAdapter.java|設定事件標籤recycler view 畫面|
|1-1-3|FriendGroupRecyclerViewAdapter.java|設定群組recycler view 畫面|
|1-1-4|FriendMemoAddColumnRecyclerViewAdapter.java|設定客製化欄位recycler view 畫面|
|1-1-5|FriendProfileListViewAdapter.java|設定朋友資訊recycler view 畫面|
|1-1-6|MatchedDeviceRecyclerViewAdapter.java|設定附近配對裝置recycler view 畫面|
|1-1-7|SelfInviteRecyclerViewAdapter.java|設定事件邀請recycler view 畫面|
|資料夾名稱:\background||
|編號|檔案名稱|功能|
|1-2-1|FriendInviteService.java|好友邀請通知發送|
|1-2-2|InviteMessageService.java|好友邀請訊息接收|
|1-2-3|NotificationService.java|附近好友通知發送|
|資料夾名稱:\bean||
|1-3-1|ActivityInviteBean.java|設定ActivityInvite屬性，提供獲取屬性和設定屬性的方法|
|1-3-2|ResponseBody.java|設定ResponseBody屬性，提供獲取屬性和設定屬性的方法|
|1-3-3|TimelineBean.java|設定Timeline屬性，提供獲取屬性和設定屬性的方法|
|資料夾名稱:\dao||
|1-4-1|UserInformationDAO.java|UserInformation資料表操作|
|1-4-2|ActivityDateDAO.java|ActivityDate 資料表操作|
|資料夾名稱:\device||
|1-5-1|MatchListener.java|附近裝置狀態操作介面|
|資料夾名稱:\device\actionhalder||
|1-6-1|BackgroundFoundActionHandler.java|背景執行找到裝置處理動作|
|1-6-2|ForegroundFoundActionHandler.java|前景執行找到裝置處理動作|
|資料夾名稱:\device\actionhalder\supplier||
|1-7-1|BackgroundActionHandlerSupplier.java|註冊背景搜尋動作|
|1-7-2|ForegroundActionHandlerSupplier.java|註冊前景搜尋動作|
|資料夾名稱:\device\beacon||
|1-8-1|BeaconSharedPreferences.java|Beacon 屬性設定|
|1-8-2|BeaconDiscoverServer.java|Beacon廣播設定|
|1-8-3|BeaconHelper.java|Beacon 搜尋設定|
|資料夾名稱:\device\beacon\finder||
|1-9-1|BeaconFinder.java|Beacon 捕捉裝置設定|
|資料夾名稱:\device\enumerate||
|1-10-1|FindAction.java|列舉裝置搜尋狀態|
|1-10-2|FindState.java|列舉藍芽狀態|
|資料夾名稱:\function||
|1-11-1|Consumer.java|單參數的函式傳遞介面|
|1-11-2|BiConsumer.java|雙參數的函式傳遞介面|
|1-11-3|Supplier.java|無參數的函式傳遞介面|
|資料夾名稱:\helper||
|1-12-1|AsyncTaskHelper.java|網路請求操作|
|1-12-2|AvatarHelper.java|頭像處理|
|1-13-3|DBHelper.java|資料庫建立|
|1-14-4|DeviceHelper.java|裝置識別碼取得|
|1-14-5|NotificationHelper.java|通知設定|
|1-14-6|PermissionHelper.java|權限設定|
|資料夾名稱:\network||
|1-15-1|AddCookiesInterceptor.java|設置請求cookies|
|1-15-2|ApiConfig.java|設定伺服器URL|
|1-15-3|ReceivedCookiesInterceptor.java|接收儲存伺服器cookies|
|1-15-4|RetrofitConfig.java|設定網路請求|
|資料夾名稱:\service||
|1-16-1|UserInformationService.java|userInformation網路請求介面|
|1-16-2|ActivityInviteService.java|activityInvite網路請求介面|
|資料夾名稱:\service\impl||
|1-17-1|UserInformationServiceImpl.java|userInformation網路請求實作|
|1-17-2|ActivityInviteServiceImpl.java|activityInvite網路請求實作|
|資料夾名稱:\activity||
|1-18-1|AddIntroductionActivity.java|註冊畫面操作|
|1-18-2|LoginActivity.java|登入畫面操作|
|1-18-3|SearchActivity.java|附近裝置搜尋畫面操作|
|1-18-4|FriendSearchActivity.java|好友列表畫面操作|
|1-18-5|FriendsTimelineActivity.java|好友時間軸畫面操作|
|1-18-6|SelfInviteActivity.java|個人邀請畫面操作|
|資料夾名稱:\fragment||
|1-19-1|EditMemoFragment.java|顯示編輯備註畫面|
|1-19-2|EditProfileFragment.java|顯示編輯客製化欄位畫面|
|1-19-3|FriendSearchAllFragment.java|顯示搜尋好友列表畫面|
|1-19-4|FriendSearchGroupFragment.java|顯示搜尋群組畫面|

    
(二)、 伺服器端

表 9-1-2 伺服器端 Project 元件清單
|資料夾名稱:|\bean||
|---|---|---|
|編號|檔案名稱|功能|
|2-1-1|ActivityDateBean.java|設定ActivityDate屬性，提供獲取屬性和設定屬性的方法|
|2-1-2|ActivityInviteBean.java|設定ActivityInvite屬性，提供獲取屬性和設定屬性的方法|
|2-1-3|ActivityLabelBean.java|設定ActivityLabel屬性，提供獲取屬性和設定屬性的方法|
|2-1-4|ActivityRemindBean.java|設定ActivityRemind屬性，提供獲取屬性和設定屬性的方法|
|2-1-5|CodeTableBean.java|設定CodeTable屬性，提供獲取屬性和設定屬性的方法|
|2-1-6|FriendBean.java|設定Friend屬性，提供獲取屬性和設定屬性的方法|
|2-1-7|FriendCustomization.java|設定FriendCustomization屬性，提供獲取屬性和設定屬性的方法|
|2-1-8|FriendGroupBean.java|設定FriendGroup屬性，提供獲取屬性和設定屬性的方法|
|2-1-9|GroupsBean.java|設定Groups屬性，提供獲取屬性和設定屬性的方法|
|2-1-10|ProblemReportBean.java|設定ProblemReport屬性，提供獲取屬性和設定屬性的方法|
|2-1-11|TimelineBean.java|設定Timeline屬性，提供獲取屬性和設定屬性的方法|
|2-1-12|UserInformationBean.java|設定UserInformation屬性，提供獲取屬性和設定屬性的方法|
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
|2-3-5|FriendController.java|控制處理前端/App請求|
|2-3-6|FriendCustomization.java|控制處理前端/App請求|
|2-3-7|FriendGroupController.java|控制處理前端/App請求|
|2-3-8|GroupsController.java|控制處理前端/App請求|
|2-3-9|ProblemReportController.java|控制處理前端/App請求|
|2-3-10|TimelineController.java|控制處理前端/App請求|
|2-3-11|UserInformationController.java|控制處理前端/App請求|
|2-3-12|RouteController.java|控制處理前端/App請求|
|資料夾名稱:|\converter||
|編號|檔案名稱|功能|
|2-4-1|LocalDateTimeConverter.java|日期轉換設定檔|
|資料夾名稱:|\dao||
|編號|檔案名稱|功能|
|2-5-1|ActivityDateDAO.java|ActivityDate資料表操作介面|
|2-5-2|ActivityInviteDAO.java|ActivityInvite資料表操作介面|
|2-5-3|ActivityLabelDAO.java|ActivityLabel資料表操作介面|
|2-5-4|ActivityRemindDAO.java|ActivityRemind資料表操作介面|
|2-5-5|CodeTableDAO.java|CodeTable資料表操作介面|
|2-5-6|FriendDAO.java|Friend資料表操作介面|
|2-5-7|FriendCustomization.java|FriendCustomization資料表操作介面|
|2-5-8|FriendGroupDAO.java|FriendGroup資料表操作介面|
|2-5-9|GroupsDAO.java|Groups資料表操作介面|
|2-5-10|ProblemReportDAO.java|ProblemReport資料表操作介面|
|2-5-11|TimelineDAO.java|Timeline資料表操作介面|
|2-5-12|UserInformationDAO.java|UserInformation資料表操作介面|
|2-5-13|BaseDAO.java|資料庫基本操作功能介面|
|資料夾名稱:|\dao\impl||
|編號|檔案名稱|功能|
|2-6-1|ActivityDateDAOImpl.java|ActivityDate資料表操作實作|
|2-6-2|ActivityInviteDAOImpl.java|ActivityInvite資料表操作實作|
|2-6-3|ActivityLabelDAOImpl.java|ActivityLabel資料表操作實作|
|2-6-4|ActivityRemindDAOImpl.java|ActivityRemind資料表操作實作|
|2-6-5|CodeTableDAOImpl.java|CodeTable資料表操作實作|
|2-6-6|FriendDAOImpl.java|Friend資料表操作實作|
|2-6-7|FriendCustomization.java|FriendCustomization資料表操作實作|
|2-6-8|FriendGroupDAOImpl.java|FriendGroup資料表操作實作|
|2-6-9|GroupsDAOImpl.java|Groups資料表操作實作|
|2-6-10|ProblemReportDAOImpl.java|ProblemReport資料表操作實作|
|2-6-11|TimelineDAOImpl.java|Timeline資料表操作實作|
|2-6-12|UserInformationDAOImpl.java|UserInformation資料表操作實作|
|2-6-13|BaseDAOImplImpl.java|資料庫基本操作功能實作|
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
|2-8-12|UserInformationService.java|UserInformation相關業務邏輯介面|
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
|2-9-12|UserInformationServiceImpl.java|UserInformation相關業務邏輯實作|
|資料夾名稱:|\utils||
|編號|檔案名稱|功能|
|2-10-1|BCryUtility.java|密碼加密、密碼比對|
|2-10-2|BeanUtility.java|更新傳入物件的屬性值|
|2-10-3|ResponseUtils.java|請求回應設定|
|資料夾名稱:|\vo||
|編號|檔案名稱|功能|
|2-11-1|ActivityDate.java|ActivityDate資料表對映|
|2-11-2|ActivityInvite.java|ActivityInvite資料表對映|
|2-11-3|ActivityLabel.java|ActivityLabel資料表對映|
|2-11-4|ActivityRemind.java|ActivityRemind資料表對映|
|2-11-5|CodeTable.java|CodeTable資料表對映|
|2-11-6|Friend.java|Friend資料表對映|
|2-11-7|FriendCustomization.java|FriendCustomization資料表對映|
|2-11-8|FriendGroup.java|FriendGroup資料表對映|
|2-11-9|Groups.java|Groups資料表對映|
|2-11-10|ProblemReport.java|ProblemReport資料表對映|
|2-11-11|Timeline.java|Timeline資料表對映|
|2-11-12|UserInformation.java|UserInformation資料表對映|
|2-11-13|CodeTablePK.java|CodeTable primary key資料表對映|
|2-11-14|UserRole.java|UserRole資料表對映|
(三)、 網頁端
|資料夾名稱:|\templates||
|---|---|---|
|3-1-1|login.html|登入頁面|
|3-1-2|logout.html|登出頁面|
|3-1-3|error403.html|http status 403 頁面|
|3-1-4|error404.html|http status 404 頁面|
|資料夾名稱:|\templates\problem_report||
|3-2-1|userReport.html|問題回報頁面|
|3-3-2|userSuccess.html|問題回報成功頁面|
|3-3-3|search.html|問題回報管理者頁面|
9-2 程式規格描述
