# Git介紹
Git是現在非常常聽到的技術之一，其主要功能為解決多人協同合作開發造成相互衝突的問題，同時也解決了在編輯文件或開發程式上版本控制的問題。也因為這個技術，讓全世界程式語言開發速度突飛猛進。  
以下這個情境也許你也發生過：同學們間一起趕一份報告，或工作團隊間大家一起合作寫一支程式。不管說好是誰改什麼地方、誰寫什麼地方，但是在最後合併時，不僅有時會搞的一團亂，甚至誰改哪邊都有機會漏掉，造成很多時間的浪費。而Git的出現，這些狀況都不復存在，這套技術就是現今每個人都必備的技術。

## 從DVCS談起

Git是一套免費開放原始碼的分散式版本控制系統 (Distributed Version Control System,DVCS)

客戶端不只能取得最後一個版本，可以向伺服器端複製完整的數據庫至本地，而當伺服器的檔案損毀時，
可以從任何一個客戶端複製資料還原到伺服器中，每次取出就是備份整個數據庫，
這就是分散式版本控制系統。

##為什麼要版本控制

版本控制是一個能夠記錄一個或一組檔案在某一段時間的變更，

使得客戶端以後能取回特定版本的系統。


##那它跟集中式版本控制系統(Centralized Version Control Systems,CVCS)比有什麼優勢呢？

1.當伺服器發生故障時，還是能本地進行作業

2.當伺服器的數據庫損毀時，其他客戶端能進行備份補救。

##那什麼是 Git 呢？

Git由 Linus Trovalds(Linux之父)  ，

為了管理Linux內核而程式碼而開發的，

在眾多的使用者評為DVCS工具中的頂級工具

且Git 是一個快速、可擴展的分布式版本控制系統。



##Git 優點：

*適合分佈式開發

*減輕伺服器壓力和數據量不會太大

*速度快

*任意兩個開發者可以容易解決衝突

*.能離線工作


##Git 缺點：

*程式碼保密性差


## 前言：
有點像是這篇文章的大綱，你這篇文章叫做「介紹Git」，對於外行人來說，想要了解的是為何需要Git，在什麼狀況下會有Git，動機目的為何。

外面有句話說得好「所謂的專業，是用別人聽得懂的話，說別人不懂的東西」

所以你這篇文章太偏操作面了，我想要的是概念。

-------------------我的心得------------------

git flow可以知道大型專案的分支使用模式，要告訴別人你會了些什麼或是告訴別人你會的東西時，最好的方法就是用情境去模擬，可以快速的讓人知道你想表達什麼，也更好理解。
這次準備的不夠充足，也說明了其實還不夠熟悉git。回家還是要多多熟悉

----bana 心得
活用git,不用想的太死,以生活化的方式理解，他是一個方便做事情的工具,我想只要工作前先,都先將檔案更新，再來開始做事情
發生衝突的機會會降更低使用上靈活  ,分散是的好處是讓大家同時開發,增加工作效率,減少開發成本
所以在我們這種要快速開發網頁的團隊中是非常必要之工具,希望大家能好好使用
我本人容易緊張，希望進度趕好學好來不要有脫隊之情形,不行的就趕快提早出來問,不要拖
會影響到整體進度，每個人計畫都要好好去實行,辛苦才是值得的


------------------相振玫的心得--------------

第一次聽到Git這個東西，真的完全沒有概念。

Google上有許多的文章，一篇一篇的看過之後，發現Git之所以好用的地方是因為branch，branch主要是用於開發專案、開發新功能，
不只是用在團隊開發，有的時候在個人作業上也可以使用。仔細想想的話，這個功能真的非常好用，想要開發新功能時，開一個分支，
做好了再合併到主線上就好；但要是做壞了也沒有關係，因為不會對你在主線上的東西造成影響。

但是，我們雖然去查了Git的特性、優缺點，去想什麼時候要用到Git，甚至也稍微的操作過Git的基本指令，
但當真的有人問我「為什麼要用Git？」我還是回答不出來，我想我對Git還不完全熟悉，這是我必須再努力，再去摸索的地方。
----------------------
Autumn.............
剛開始接觸Git的時候，查了一些資料還有夥伴們所寫的文章，還是不太清楚是在做什麼，
在打指令的時候，邊下指令邊去了解這個指令的實際用法，雖然還有些基本的還不是很了解，所以短時間內要把這些不熟悉的部分，盡快理解上手並了解那些指令在什麼時候使用
或許學習的速度會比其他夥伴來的慢，但是有問題大家會一起想辦法，這種一起成長一起進步的感覺，是前所未有的。

-----test message----

Donec sed odio dui. Maecenas sed diam eget risus varius blandit sit amet non magna. Aenean lacinia bibendum nulla sed consectetur. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Curabitur blandit tempus porttitor. Donec ullamcorper nulla non metus auctor fringilla.

Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit. Nullam id dolor id nibh ultricies vehicula ut id elit. Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit sit amet non magna.

Donec sed odio dui. Aenean lacinia bibendum nulla sed consectetur. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Sed posuere consectetur est at lobortis. Nullam quis risus eget urna mollis ornare vel eu leo. Sed posuere consectetur est at lobortis.

Maecenas sed diam eget risus varius blandit sit amet non magna. Maecenas sed diam eget risus varius blandit sit amet non magna. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Maecenas faucibus mollis interdum. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Vestibulum id ligula porta felis euismod semper.
>>>>>>> bd9a92f0354f24caf32e6eaef2245608c8667b71
