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


 ## git init 、git add . 、 git commit -m "your message" 操作篇

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.開啟 Git Shell
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![08](https://github.com/a65162/Git-Learnig/blob/master/img/08.jpg)
