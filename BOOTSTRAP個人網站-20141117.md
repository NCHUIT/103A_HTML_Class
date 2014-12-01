BOOTSTRAP X GITHUB PAGE (20141117)
====

CREATE A PERSONAL WEBSITE

[SlideShare][1]

Things worth sharing
----
![Google Student Pack][12]
[使用中興大學申請 Google 帳號獲得學生獨享優惠][2]

GIT
----

中文全名：分散式版本控制管理系統

為何要使用 GIT
----

![寫程式？那些老師沒教的事][13]
**[寫程式？那些老師沒教的事][3]**
> 請看以上投影片的 p42 ~ p106

用 GIT 取回程式碼
----

> 使用 TortoiseGit 抓回 GitHub 上的程式碼

  - 打開專案頁面
  - 複製 SSH clone URL (git@github.com:XXX.git)
  - 開啟「C:\xampp\htdocs」
  - 右鍵選擇「Git Clone…」

![RightClick][14]
  - URL貼上剛剛複製的
  - SSH clone URL
  - Load Putty Key 選擇第一次上課建立的私鑰 .ppk
  - 按下OK，開始 clone
  - 有需要私鑰密碼的話記得輸入

確認取回成功
----
  - 開啟 Google Chrome，連線至"http://localhost/"…
  - 確認網頁成功顯示
  - 記得開啟XAMPP伺服器 XAMPP Control Panel(C:\xampp\xampp-control.exe)

GIT COMMIT
----

如果有修改任何程式碼，記得要 COMMIT 和 PUSH
這樣才會有版本管理的效果

No ~~save~~, no ~~load~~.
----

  - 右鍵「Git Commit → master」
  - 選擇要存檔的檔案
  - 打入以後給自己看的說明
  - 按下「OK」
  - 記得「Push」回Github

![Git Commit][15]

Push to Github
----
  - 右鍵選單選「Push」
  - ![Git Push][16]
  - 推送到「Origin」的「master」分支。(預設是這個)
  - ![Git Push][17]

Bootswatch
----
網站跟別人一樣，~~小心勝文不開心~~

[BootsWatch][4]

還有付費的樣式 {wrap}boostrap

[WrapBootstrap][5]


PERSONAL WEBSITE
----

其實跟寫自傳很像啦

Yes123 自傳建議
![Yes123自傳建議][18]

個人網站內容範例
----

  - Taichunmin - [Link][6]
  - Morris821028 - [Link][7]
  - 蒼時弦也 - [Link][8]
  - 下一位...


**請用 ``site:http://github.io`` 選擇繁體中文來搜尋範例**

![github.io example Search][19]

互評標準
----

  - 整齊的程式碼縮排
  - Bootstrap套用正確
  - 首頁xs瀏覽正常
  - 首頁sm瀏覽正常
  - 首頁md瀏覽正常
  - 首頁lg瀏覽正常
  - 網站內包含圖片``<img>``
  - 選單在各種大小運作正常
  - 套用一個別人的 Bootstrap Theme

我有問題該問誰？
----

  - [均民][9]
  - [冠喻][10]
  - [川哲][11]

**記得作網站~不要裝死XD**

[]: "Links"
[1]: http://goo.gl/qXDYuL "SlideShare"
[2]: http://goo.gl/dXIyeE "Pastleo's guide for google student account"
[3]: http://www.slideshare.net/taichunmin/ss-16096723 "Git介紹"
[4]: http://bootswatch.com/ "BootsWatch"
[5]: https://wrapbootstrap.com/ "WrapBootstrap"
[6]: http://taichunmin.idv.tw/ "taichunmin's page"
[7]: http://morris821028.github.io/ "Morris831028's page"
[8]: http://frost.tw/ "蒼時弦也's page"
[9]: http://facebook.com/taichunmin "taichunmin's facebook"
[10]: http://facebook.com/ChiuGuanYu "pastleo's facebook"
[11]: http://facebook.com/CJHwong "CJHwong's facebook"

[]: "Images"
[12]: media/20141117/image4.png
[13]: media/20141117/image6.jpg
[14]: media/20141117/image8.png
[15]: media/20141117/image11.png
[16]: media/20141117/image12.png
[17]: media/20141117/image13.png
[18]: media/20141117/image15.png
[19]: media/20141117/image16.png