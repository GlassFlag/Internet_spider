#在init_code里。实现了爬取保存一个网页。但是问题是。每次都要自己手动去输入要保存的网址还不如自己一个个动手去保存了。
#然而作为懒人我是死都不要做这种蠢事。所以在第一次迭代里。需要添加的功能：
#1.分析html，得出页面中的URL。然后一个一个页面的自动去爬取保存。
#但是现在问题来了。万一两个页面互相有URL。这样不就是一个死循环了么，我都不忍心看这蠢蠢的spider来回爬了
#为了解决以上问题。我们必须添加一个数据结构用来储存之前爬过的url
#2.建立一个数据结构保存爬过的url。然后什么算法的复杂度啦分析啦。学过的又可以用上啦~自己去拓展哦。选取最好的数据结构和算法
#3.写HTTP协议的报头。

import os
import urllib.request

path = 'D:\\Internet_Spider\\webpage.html'
def save_page(data):
	f_obj = open(path,'wb')
	f_obj.write(data)
	f_obj.close()
	print('ok')
weburl = 'http://www.douban.com'
#问我报头是怎么知道的？1.看《HTTP权威指南》。2.用Fidder（抓包工具）
webheaders = {'User-Agent: Mozilla/5.0 (Windows NT 6.3; WOW64; rv:42.0) Gecko/20100101 Firefox/42.0'}
#构造报头
req = urllib.request.Request(url = weburl, headers = webheaders)
webpage = urllib.request.urlopen(req)       #这里注意和init_code区别。在init_code里参数是URL。这里发送的是报头。
data = webpage.read()


save_page(data)

