import urllib
import urllib.request
import os

path = 'D:\\Internet_Spider\\webpage.html'
def save_page(data):
	f_obj = open(path,'wb')
	f_obj.write(data)
	f_obj.close()
	print('ok')
url = 'http://www.douban.com'
url = urllib.parse.urlencode(url)
webpage = urllib.request.urlopen(url)
data = webpage.read()

save_page(data)
