#!usr/bin/env python
# -*- encoding:utf-8 -*-

# @name  : 12306py
# @author: tian
# @date  : 2018/3/19 0019
# @des   : '''获取车站对应词典'''

import requests
import re

requests.packages.urllib3.disable_warnings()
# 12306的城市名和城市代码js文件url
url = 'https://kyfw.12306.cn/otn/resources/js/framework/station_name.js?station_version=1.9080'
r = requests.get(url,verify=False)
pattern = u'([\u4e00-\u9fa5]+)\|([A-Z]+)'
result = re.findall(pattern,r.text)
station = dict(result)
print(station)
# url = "https://kyfw.12306.cn/otn/resources/merged/queryLeftTicket_end_js.js?scriptVersion=1.9080"
