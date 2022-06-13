# 投票作業系統
## 使用者故事(user story)

### 首頁

* 進入首頁
 * 可以看見正在進行的投票(不記名)
   包含投票到期日
 * 可以看見已經結束的投票(不記名)
   將結果已縮圖的方式顯示
 * 投票結果  
 * 登入窗口
 * 註冊窗口
### 使用者端

* 註冊窗口
 * 註冊會員需要(帳號 姓名 性別 生日 學歷 住址 身分證 信箱 手機 密碼 再次確認的密碼 驗證碼)
 * 確定按鈕 重填按鈕
   * 確定後跳入後台驗證 
      * 如果正確 跳出註冊成功(信箱驗證?) 回首頁按鈕
      * 如果錯誤 將有問題的項目反紅
   * 重填後重新導入註冊頁面 然後洗掉舊有資料

* 登入窗口
  * 登入成功 跳入會員中心
  * 登入失敗 跳出登入失敗 如果沒有會員請先註冊

* 會員中心
  * 可以看見正在進行的投票(記名+不記名)
  * 可以看見已經結束的投票(記名+不記名)
  * 已發起的投票(刪除按鈕)
  * 查看參與過的投票
  * 發起投票按鈕

* 設計投票的頁面
  * 新增題目
  * 刪除題目
  * 設定選項

* 投票結果
  * 顯示結果的統計資料

### 管理者端
* 會員資料按紐
* 所有投票按鈕

* 會員資料中心
  * 可以管理所有會員資料(刪除)

* 所有投票
  * 可以管理所有投票(刪除 更改)

## 功能需求
* 註冊/登入系統
* 頁面切版
* 前端讀出功能(列表/註冊列表/會員中心)
* 投票系統(新增/刪除/修改)
* 投票結果的統計分析
* 投票參與者資料分析

## 資料表設計
### 資料庫名稱:vote
* user
   |名稱|型態|預設值|A_I|備註| 
   |ID|int(11)|--|ture|序號|
   |帳號(acc)|varchar(12)|--|--|帳號|
   |密碼(pw)|varchar(16)|--|--|--|
   |姓名(name)|varchar(12)|--|--|--|
   |性別(gender)|tinyint(1)|--|--|--|
   |生日(birthday)|date|--|--|--|
   |學歷(eduction)|varchar(32)|--|--|--|
   |住址(addr)|varchar(64)|--|--|--|
   |身分證(idcard)|varchar(12)|--|--|--|
   |信箱(e-mail)|varchar(64)|--|--|--|
   |手機(phone)|varchar(12)|--|--|--|
