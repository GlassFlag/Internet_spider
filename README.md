# Internet_spider
python 3.5

地图迭代学习法

##init_code
回忆下python的语法

os模块关于文件的操作函数

代码报错的可能性。path变量保存的是我的系统里存在的路径，如果你的D盘没有Internet_Spider这个文件夹的话，程序会出错，后面会支持修改路径的。

##第一次迭代GET：
需要点亮的技能点：HTTP协议-报头。数据结构：队列和集。一点点的正则
----
在init_code里。实现了爬取保存一个网页。但是问题是。每次都要自己手动去输入要保存的网址还不如自己一个个动手去保存了。
然而作为懒人我是死都不要做这种蠢事。所以在第一次迭代里。需要添加的功能：

1.分析html，得出页面中的URL。然后一个一个页面的自动去爬取保存。但是现在问题来了。万一两个页面互相有URL。这样不就是一个死循环了么，我都不忍心看这蠢蠢的spider来回爬了。<(￣︶￣)>为了解决以上问题。我们必须添加一个数据结构用来储存之前爬过的url。

2.建立一个数据结构保存爬过的url。然后什么算法的复杂度啦分析啦。学过的又可以用上啦~自己去拓展哦。选取最好的数据结构和算法。不会的快去复习。

3.最后的问题就是，万一服务器学精了。知道你这是一只spider拒绝‘浪费流量’给你数据怎么办？那之前写的一大堆不是废了么。绝对不允许做无用功。所以现在的问题就是，怎么把你的spider画一个漂亮的妆让它看起来就是一个客户端（浏览器）的请求。这里用到了HTTP协议的细节。

-----
等你完成了第一次迭代就会发现，你的技能又多会了几个！
##第二次迭代GET：
正则表达式
