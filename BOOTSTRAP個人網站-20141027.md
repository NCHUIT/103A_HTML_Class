BOOTSTRAP X GITHUB PAGE (20141027)
====

CREATE A PERSONAL WEBSITE

[SlideShare][1]

HTML5 已正式發布
----
2014/10/28 - [Link][2]
![][25]

安裝 xampp
----
  - [官方網站][3]
  - 安裝後，以系統管理員開啟 Xampp Control Panel
  - 將 Apache 和 MySQL 設定為開機自動開啟
  - 連線到 ``http://127.0.0.1/`` 或 ``http://localhost/`` 驗證安裝成功

**Step 1. 安裝XAMPP，只需要安裝這些東西就行了**

![][26]

**Step 2. 用 XAMPP control panel 開啟 apache 和 mysql**

![][27]

**Step 3. Localhost 或是 127.0.0.1**

![][28]

**Step 4. 直接從 github 新增檔案到 repo**

![][29]

**Step 5. 新增檔案**

![][30]

**Step 6. 修改檔案**

![][31]

Personal Website Viewer
----

![][32]

HTML + bootstrap 基礎
----
[Bootstrap Website][4]

HTML 初始程式碼
----

  - L1：HTML5的宣告
  - L2：``<html>``標籤，萬物起源
  - L3：``<head>``標籤，HTML的描述
  - L4：``<meta charset="…">``HTML文件的編碼方式
  - L5：文件的標題
  - L7：``<body>``標籤，文件的內容

![][33]

HTML標籤
----

![][34]

> 標籤名稱： div  
> 標籤內容： hello world  
> 標籤屬性：id="news-1" class="article"

Html entities
----

![][35]


超連結 ``<a>…</a>``
----

  - 連結到絕對網址
``<a href="http://www.google.com.tw/">Google</a>``

  - 連線到相對網址
``<a href="test/index.html">index</a>``

  - 書籤
``<a href="#content">content</a>``

套用 Bootstrap
----

![][36]

> Line 06:在head標籤最底下套用Bootstrap的CSS  
> Line 09:在body標籤最底下先套用jQuery  
> Line 10:然後再套用bootstrap的javascript  

[Bootstrap CDN][5], [jQuery on Google CDN][6]

為了瀏覽器及手機的相容性，加上額外的head資訊
----

[參考網址][7]

![][37]

手機瀏覽兩三事
----

  - 為了讓手機瀏覽器知道網頁有為手機設計，可加上 viewport

```html
    <meta name="viewport" content="width=device-width, initial-scale=1">
```

  - 如果希望在手機上面禁止縮放，可限制縮放倍率

```html
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
```

[詳細說明][8]

Bootstrap 樣式
----

[Link][9]

Bootstrap的網頁容器
----
  - 使用 Bootstrap 時需要將內容放進容器，才有辦法使用 Grid system 和把網頁內容置中
  - 注意：不要巢狀套用，不然排版會怪怪的
  - 使用 .container 來作為自適應容器

```html
    <div class="container">
        ...
    </div>
```

  - 使用 .container-fluid 來作為 100% 寬度的容器

```html
    <div class="container-fluid">
        ...
    </div>
```

Grid system 網格系統
----

在 Bootstrap 內有一個簡單、自適應 (responsive)、行動優先 (mobile first) 的 Grid 系統，頁面會被 Grid 系統分成 12 行，當螢幕大小改變時，可以跟著改變資料所佔的行數。

**Grid System 分成四種寬度**
  - Extra small 手機 ( < 768px )
  - Small 直向平板 ( >= 768px )
  - Medium 橫向平板 ( >= 992px )
  - Large 桌上型螢幕 ( >= 1200px )

![][38]

[詳細資料][11]

頁面布局
----

1-1 欄寬

![][39]

1-1-1 欄寬

![][40]

2-1 欄寬

![][41]

[多種欄寬方式][12]、[巢狀 Grid 系統][13]

Html heading
----

```html
<h1>我是h1標籤</h1>
<h2>我是h2標籤</h2>
<h3>我是h3標籤</h3>
<h4>我是h4標籤</h4>
<h5>我是h5標籤</h5>
<h6>我是h6標籤</h6>
```

![][42]

[詳細資料][14]

文字段落 ``<p>…</p>``
----

![][43]

行內裝飾
----

  - 標記 ``<mark>…</mark>``

![][44]

  - 刪除線 ``<del>…</del>``、``<s>…</s>``

![][45]

  - 底線 ``<ins>…</ins>``、``<u>…</u>``

![][46]

  - 縮小字體 ``<small>…</small>``

![][47]

  - 粗體 ``<strong>…</strong>``

![][48]

  - 斜體 ``<em>…</em>``

![][49]

文字排列
----

![][50]

**Try it yourself**

請用愛用 [亂數假文產生器][15]

無序清單
----

![][51]

有序清單
----

![][52]

無樣式的清單
----

![][53]

表格
----

```html
    <div class="container">
        <h1>Hello, world!</h1>
        <table class="table table-borded table-striped">
            <tr class="info">
                <th>XOR</th>
                <th>True</th>
                <th>False</th>
            </tr>
            <tr>
                <th class="info">True</th>
                <td>False</td>
                <td>True</td>
            </tr>
            <tr>
                <th class="info">False</th>
                <td>True</td>
                <td>False</td>
            </tr>
        </table>
    </div>
```
![][54]

bootstrap表格
----

在一般的 html 表格加上 .table 就可套用 Bootstrap 的樣式

![][55]

[詳細資料][16]

自適應表格 (responsive)
----

![][56]

[詳細資料][17]

表單 (跳過)
----

因為個人網站用不到表單 (form)，歡迎私下詢問。([文件在此][18])

按鈕 ``<a> <button> <input>``
----

![][57]

[詳細資料][19]

圖片
----

  - 為了讓圖片也可以自適應螢幕大小，故須加上 .img-responsive

```html
<img src="..." class="img-responsive"></img>
```

  - 圖片裝飾

![][58]

記得看過被我略過的東西
----
> 因為時間不夠，所以就自己看囉~
> [Link][9]

Bootstrap組件
----

[Link][21]

Glyphicons 圖案
----

![][59]

[詳細資料][22]

navbar
----

![][60]

```html
<nav class="navbar navbar-default" role="navigation">
  <div class="container-fluid">
    <!-- Brand and toggle get grouped for better mobile display -->
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">Brand</a>
    </div>
    <!-- Collect the nav links, forms, and other content for toggling -->
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
      <ul class="nav navbar-nav">
        <li class="active"><a href="#">Link <span class="sr-only">(current)</span></a></li>
        <li><a href="#">Link</a></li>
        <li class="dropdown">
          <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-expanded="false">Dropdown <span class="caret"></span></a>
          <ul class="dropdown-menu" role="menu">
            <li><a href="#">Action</a></li>
            <li><a href="#">Another action</a></li>
            <li><a href="#">Something else here</a></li>
            <li class="divider"></li>
            <li><a href="#">Separated link</a></li>
            <li class="divider"></li>
            <li><a href="#">One more separated link</a></li>
          </ul>
        </li>
      </ul>
      <form class="navbar-form navbar-left" role="search">
        <div class="form-group">
          <input type="text" class="form-control" placeholder="Search">
        </div>
        <button type="submit" class="btn btn-default">Submit</button>
      </form>
      <ul class="nav navbar-nav navbar-right">
        <li><a href="#">Link</a></li>
        <li class="dropdown">
          <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-expanded="false">Dropdown <span class="caret"></span></a>
          <ul class="dropdown-menu" role="menu">
            <li><a href="#">Action</a></li>
            <li><a href="#">Another action</a></li>
            <li><a href="#">Something else here</a></li>
            <li class="divider"></li>
            <li><a href="#">Separated link</a></li>
          </ul>
        </li>
      </ul>
    </div><!-- /.navbar-collapse -->
  </div><!-- /.container-fluid -->
</nav>
```

[詳細資料][23]

panel
----

![][61]

```html
<div class="panel panel-default">
  <div class="panel-heading">Panel heading without title</div>
  <div class="panel-body">
    Panel content
  </div>
</div>

<div class="panel panel-default">
  <div class="panel-heading">
    <h3 class="panel-title">Panel title</h3>
  </div>
  <div class="panel-body">
    Panel content
  </div>
</div>
```


[詳細資料][24]

[]: "Links"
[1]: http://goo.gl/W1NfUW "SlideShare"
[2]: http://www.w3.org/TR/html5/ "html5"
[3]: https://www.apachefriends.org/zh_tw/index.html "xampp"
[4]: http://getbootstrap.com/ "Bootstrap Website"
[5]: http://getbootstrap.com/getting-started/#download-cdn "Bootstrap CDN"
[6]: https://developers.google.com/speed/libraries/devguide?hl=zh-tw#jquery "jQuery on Google CDN"
[7]: http://getbootstrap.com/getting-started/#template "browser and mobile support"
[8]: http://getbootstrap.com/css/#overview-mobile "mobile viewport"
[9]: http://getbootstrap.com/css/ "Bootstrap CSS"
[10]: http://getbootstrap.com/css/#overview-container "container"
[11]: http://getbootstrap.com/css/#grid "Grid System"
[12]: http://getbootstrap.com/css/#grid-example-mixed-complete "Grid Mix column"
[13]: http://getbootstrap.com/css/#grid-nesting "Grid Nesting"
[14]: http://getbootstrap.com/css/#type-headings "Headings"
[15]: http://www.richyli.com/tool/loremipsum/ "亂數假文產生器"
[16]: http://getbootstrap.com/css/#tables "Tables"
[17]: http://getbootstrap.com/css/#tables-responsive "Responsive Tables"
[18]: http://getbootstrap.com/css/#forms "Forms"
[19]: http://getbootstrap.com/css/#buttons "Buttons"
[20]: http://getbootstrap.com/css/#images "Images"
[21]: http://getbootstrap.com/components/ "Components"
[22]: http://getbootstrap.com/components/#glyphicons "Glyphicons"
[23]: http://getbootstrap.com/components/#navbar "NavBar"
[24]: http://getbootstrap.com/components/#panels "Panels"



[]: "Images"
[25]: media/20141027/image2.png
[26]: media/20141027/image3.png
[27]: media/20141027/image4.png
[28]: media/20141027/image5.png
[29]: media/20141027/image6.png
[30]: media/20141027/image7.png
[31]: media/20141027/image8.png
[32]: media/20141027/image9.png
[33]: media/20141027/image10.png
[34]: media/20141027/image11.png
[35]: media/20141027/image12.png
[36]: media/20141027/image13.png
[37]: media/20141027/image14.png
[38]: media/20141027/image19.png
[39]: media/20141027/image20.png
[40]: media/20141027/image21.png
[41]: media/20141027/image22.png
[42]: media/20141027/image24.png
[43]: media/20141027/image25.png
[44]: media/20141027/image26.png
[45]: media/20141027/image27.png
[46]: media/20141027/image28.png
[47]: media/20141027/image29.png
[48]: media/20141027/image30.png
[49]: media/20141027/image31.png
[50]: media/20141027/image32.png
[51]: media/20141027/image33.png
[52]: media/20141027/image34.png
[53]: media/20141027/image35.png
[54]: media/20141027/image37.png
[55]: media/20141027/image38.png
[56]: media/20141027/image39.png
[57]: media/20141027/image40.png
[58]: media/20141027/image41.png
[59]: media/20141027/image42.png
[60]: media/20141027/image43.png
[61]: media/20141027/image45.png
