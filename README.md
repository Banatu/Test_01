# Git


## 前言

   &nbsp;&nbsp;&nbsp;&nbsp;Git是從2005年創立的開源分散式版本控制系統，由Linus Torvalds創作，為了幫助管理Linux內核開發而開發出來的開源軟體。<br/>
   &nbsp;&nbsp;&nbsp;&nbsp;當初全世界Linux開發人員所使用的BitKeeper屬於私人軟體，在開放源社區上遭他人反對認為BitKeeper的軟體並不適合在開放源社區的工作，所以Linus Torvalds決定開始著手開發比BitKeeper還要好的版本控制系統，雖然最初目的是為了管理Linux內核的開發，但是後來發現很多自由軟體也使用了Git 。

<br/><br/><br/>
## 什麼時候使用Git?

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.方便查詢過去更改的紀錄內容

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.可以隨意復原之前的紀錄內容

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.多人合作開發時，不會覆蓋到別人的東西

<br/><br/><br/>
## 安裝Git GUI篇

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;這邊以Windows下安裝為範例

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.請至https://desktop.github.com/ 下載GUI 介面

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![01](https://github.com/a65162/Git-Learnig/blob/master/img/01.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.下載後並開啟安裝檔

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![02](https://github.com/a65162/Git-Learnig/blob/master/img/02.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. 請按Install

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![03](https://github.com/a65162/Git-Learnig/blob/master/img/03.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![04](https://github.com/a65162/Git-Learnig/blob/master/img/04.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4. 在安裝完成後程式會自動開啟<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;* 此步可以選擇登入或是點選Skip setup

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![05](https://github.com/a65162/Git-Learnig/blob/master/img/05.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5.在任何Git工具中都必須設定user.name 和 user.email 沒有這兩個參數 日後無法commit

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![06](https://github.com/a65162/Git-Learnig/blob/master/img/06.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.設定完成

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![07](https://github.com/a65162/Git-Learnig/blob/master/img/07.jpg)

> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ps.GitHub for Windows 裝好之後，其實還額外幫你安裝了一個 Git Shell 工具，這預設是一個
 PowerShell 介面的操作環境，好處有很多，之後我們的例子也會盡量使用 Git Shell 來進行操作

<br/><br/><br/>

 ## git init

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.開啟 Git Shell

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![08](https://github.com/a65162/Git-Learnig/blob/master/img/08.jpg)

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.開啟後出現的視窗

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![09](https://github.com/a65162/Git-Learnig/blob/master/img/09.jpg)

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.請創一個資料夾 並進入此資料夾 指令如下

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![10](https://github.com/a65162/Git-Learnig/blob/master/img/10.jpg)

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.本案例要管理abc資料夾  在命令次元下輸入 git init

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![11](https://github.com/a65162/Git-Learnig/blob/master/img/11.jpg)
  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;當底下出現Master時 表示已成功管理此資料夾

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5.我們在abc資料夾下創建一個記事本

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![12](https://github.com/a65162/Git-Learnig/blob/master/img/12.jpg)

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7.在命令次元下 輸入 git status ，Git會告訴你當下有一個New Text Document.txt 的檔案還未加入
   Staging area

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![13](https://github.com/a65162/Git-Learnig/blob/master/img/13.jpg)  

  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ps.<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在Git中有分三個工作區塊<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Working Directory: 所有的修改、變動都發生在這個階段。(本地的資料夾)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Staging area: 作為一個中繼的工作區，在將檔案放入資料庫之前做確認及檢查的                       工作區，確認無誤後就可以將檔案轉移至資料庫。 (當執行git add . 會使用到)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Repository: 資料庫，儲存著更新的 commit，而線上資料庫會和本機的這個區域進行同步。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8.輸入 git add . 把此檔案新增到Staging area 此時再輸入git status ，Git 會告訴你 New Text Document.txt 可以commit  

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![14](https://github.com/a65162/Git-Learnig/blob/master/img/14.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;9.輸入 git commit -m "add file"  就成功完成更新 本地的Repository

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![15](https://github.com/a65162/Git-Learnig/blob/master/img/15.jpg)

>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ps. git commit -m "your message"   your message :寫下更新的重點

<br/><br/><br/>
## Git clone 操作篇

&nbsp;&nbsp;&nbsp;&nbsp;Git clone 的目的是要複製遠端的Repository  
&nbsp;&nbsp;&nbsp;&nbsp;本教學以GitHub為例  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.先連至 https://github.com/  並在Search GitHub 搜尋 css

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![16](https://github.com/a65162/Git-Learnig/blob/master/img/16.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.我們以 https://github.com/hakimel/css 來舉例 請點選 Clone or download 的按鈕
複製出現的網址

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![17](https://github.com/a65162/Git-Learnig/blob/master/img/17.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.請打開 GitShell 輸入以下指令 它會下載在GitHub資料夾下

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![18](https://github.com/a65162/Git-Learnig/blob/master/img/18.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.瀏覽剛剛下載的專案 當有出現時表示成功clone別人的Repository

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![19](https://github.com/a65162/Git-Learnig/blob/master/img/19.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![20](https://github.com/a65162/Git-Learnig/blob/master/img/20.jpg)

<br/><br/><br/>

## git push 操作篇

&nbsp;&nbsp;&nbsp;&nbsp;push 的目的是將本地的Repository 上傳至遠端的Repository

&nbsp;&nbsp;&nbsp;&nbsp;以下教學以GitHub為例

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.請連至https://github.com/ ，請點選New Repository

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![21](https://github.com/a65162/Git-Learnig/blob/master/img/21.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.將Repository name 命名為abc，並點下Create Repository

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![22](https://github.com/a65162/Git-Learnig/blob/master/img/22.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.此視窗是建立好的畫面

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![23](https://github.com/a65162/Git-Learnig/blob/master/img/23.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.在 git init 、git add . 、 git commit -m "your message" 操作篇 中 已經完成了一個專案 以此專案為例push到遠端的Repository

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![24](https://github.com/a65162/Git-Learnig/blob/master/img/24.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5.首先我們要先建立 連接遠端必要指令 如下

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![25](https://github.com/a65162/Git-Learnig/blob/master/img/25.jpg)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![26](https://github.com/a65162/Git-Learnig/blob/master/img/26.jpg)

>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ps. git remote add "name" "position" name:可以由開發者自行命名 position:遠端專案所在的位置

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.檢查是否有建立成功 如圖下

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![27](https://github.com/a65162/Git-Learnig/blob/master/img/27.jpg)

>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ps.有出現abc 表示建立成功

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7.建立好連線時 開始要push 至遠端的Repository 如圖下

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![28](https://github.com/a65162/Git-Learnig/blob/master/img/28.jpg)

>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ps. git push "name" "branch" name在上一個步驟時以命名為abc 。branch 依照你要上傳的branch而定

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8.看看剛剛GitHub所創的abc Repository 是否有出現資料了

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![29](https://github.com/a65162/Git-Learnig/blob/master/img/29.jpg)
