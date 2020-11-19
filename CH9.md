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
|1-3-1|ResponseBody.java|設定ResponseBody屬性，提供獲取屬性和設定屬性的方法|
|1-3-2|TimelineBean.java|設定Timeline屬性，提供獲取屬性和設定屬性的方法|
|資料夾名稱:\dao||
|1-4-1|UserInformationDAO.java|UserInformation資料表操作|
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
|資料夾名稱:\network||
|1-15-1|AddCookiesInterceptor.java|設置請求cookies|
|1-15-2|ApiConfig.java|設定伺服器URL|
|1-15-3|ReceivedCookiesInterceptor.java|接收儲存伺服器cookies|
|1-15-4|RetrofitConfig.java|設定網路請求|
|資料夾名稱:\service||
|1-16-1|UserInformationService.java|userInformation網路請求介面|
|資料夾名稱:\service\impl||
|1-17-1|UserInformationServiceImpl.java|userInformation網路請求實作|
|資料夾名稱:\activity||
|1-18-1|LoginActivity.java|登入畫面操作|
|1-18-2|SearchActivity.java|附近裝置搜尋畫面操作|
|1-18-3|FriendSearchActivity.java|好友列表畫面操作|
|1-18-4|FriendsTimelineActivity.java|好友時間軸畫面操作|
|1-18-5|SelfInviteActivity.java|個人邀請畫面操作|
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
|2-1-1|TimelineBean.java|設定Timeline屬性，提供獲取屬性和設定屬性的方法|
|資料夾名稱:|\config||
|編號|檔案名稱|功能|
|2-2-1|SecurityConfig.java|登入設定檔|
|資料夾名稱:|\controller||
|編號|檔案名稱|功能|
|2-3-1|TimelineController.java|控制處理前端/App請求|
|資料夾名稱:|\converter||
|編號|檔案名稱|功能|
|2-4-1|LocalDateTimeConverter.java|日期轉換設定檔|
|資料夾名稱:|\dao||
|編號|檔案名稱|功能|
|2-5-1|FriendGroupDAO.java|FriendGroup資料表操作介面|
|2-5-3|BaseDAO.java|資料庫基本操作功能介面|
|資料夾名稱:|\dao\impl||
|編號|檔案名稱|功能|
|2-6-1|FriendGroupDAOImpl.java|FriendGroup資料表操作實作|
|2-6-2|BaseDAOImplImpl.java|資料庫基本操作功能實作|
|資料夾名稱:|\filter||
|編號|檔案名稱|功能|
|2-7-1|CustomAuthenticationSuccessHalder.java|登入成功回傳資料設定|
|2-7-2|CustomAuthenticationToken.java|保存請求參數|
|2-7-3|CustomEntryPoint.java|未登入處理設定|
|2-7-4|CustomerAccessDeniedHalder.java|權限不足回傳資料設定|
|2-7-5|CustomLoginFilter.java|登入驗證|
|資料夾名稱:|\service||
|編號|檔案名稱|功能|
|2-8-1|FriendService.java|Friend相關業務邏輯介面|
|資料夾名稱:|\service\impl||
|編號|檔案名稱|功能|
|2-9-1|FriendServiceImpl.java|Friend相關業務邏輯實作|
|資料夾名稱:|\utils||
|編號|檔案名稱|功能|
|2-10-1|BCryUtility.java|密碼加密、密碼比對|
|2-10-2|BeanUtility.java|更新傳入物件的屬性值|
|2-10-3|ResponseUtils.java|請求回應設定|
|資料夾名稱:|\vo||
|編號|檔案名稱|功能|
|2-11-1|Friend.java|Friend資料表對映|
(三)、 網頁端
|資料夾名稱:|\templates||
|---|---|---|
|3-1-1|login.html|登入頁面|
|3-1-2|error404.html|http status 404 頁面|
|資料夾名稱:|\templates\problem_report||
|3-2-1|userReport.html|問題回報頁面|
|3-3-2|userSuccess.html|問題回報成功頁面|
|3-3-3|search.html|問題回報管理者頁面|
9-2 程式規格描述
