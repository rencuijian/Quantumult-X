# Quantumult X个人查找使用教程
* 随缘编辑
# 目录
* 关于去广告
* Quantumult X详细教学
  - 小白教学
  - 大佬教学

* 关于策略组
  - 策略组的个人理解
* 关于分流  
  - 关于分流个人理解
* 关于重写
  - 重写个人理解
  
* 关于MitM
  -个人理解
* 工具&分析
  -构造HTTP请求
* 关于去广告





# 大佬链接
[blackmatrix7圈X](https://github.com/blackmatrix7/ios_rule_script)、[DivineEngine神机圈X](https://github.com/DivineEngine/Profiles/tree/master)、[NobyDa野比圈X和JS](https://github.com/NobyDa/Script)、
[chavyleung的JS安装](https://github.com/chavyleung/boxjs-doc)、[LGTMXD神机规则备份](https://github.com/LGTMXD/Profiles-1)、[lhie1](https://github.com/lhie1)、[sve1r规则排序广告释义](https://github.com/sve1r/Rules-For-Quantumult-X)

# Quantumult X参数
* KOP-XIAO的各参数说明：https://github.com/KOP-XIAO/QuantumultX/blob/master/QuantumultX_Profiles.conf
* 野比NobyDa的规则理解：https://github.com/NobyDa/Profiles
* F大的wiki策略组理解：https://github.com/Fndroid/jsbox_script/wiki/关于策略组的理解
* svelr 的规则理解：https://github.com/sve1r/Rules-For-Quantumult-X/
* 万事屋转载规则理解：https://merlinblog.xyz/wiki/rules.html


# 大佬教Quantumult X使用教程
## 小白指南(懒人教程)
* 优质盒子使用教程：https://uzbox.com/tech/quantumult-x.html?amp=1
* kjfx教程github：https://github.com/kjfx/QuantumultX
* 毒奶github：https://github.com/limbopro/Profiles4limbo
* Yatta漫游小镇：https://yattazen.com/tutorial/quantumultx-config-guide.html
* Sabrina的QuanX不求人手册:https://merlinblog.xyz/wiki/quanx.html

## 进阶指南
* [@Shawn提供的不完全指南](https://www.notion.so/Quantumult-X-1d32ddc6e61c4892ad2ec5ea47f00917) 
* [@毒奶提供的详细教程](https://limbopro.com/archives/3846.html)
* [耳东橙的教程](https://github.com/erdongchanyo/Rules/tree/main/QuantumultX)
* 优质盒子教程：https://uzbox.com/tech/quanx.html?amp=1

# 分流规则与重写库
* blackmatrix7的库: https://github.com/blackmatrix7/ios_rule_script
* 神机规则新库:https://github.com/DivineEngine/Profiles/tree/master
* Orz3的库：https://github.com/Orz-3/QuantumultX

# 图标库
    - Qure 图标库：https://github.com/Koolson/Qure
    - Mini 图标库：https://github.com/Orz-3/mini

# 去广告教程规则
* 毒奶去广告github教程：https://github.com/limbopro/Adblock4limbo
* 野比NobyDa去广告github教程：https://github.com/NobyDa/ND-AD


# Task任务京东、爱奇艺、快看漫画等签到库
* Orz3收集各博主脚本：https://github.com/Orz-3/QuantumultX/tree/master/Task
* 野比NobyDa JS脚本：https://github.com/NobyDa/Script/tree/master



# BoxJs使用方法(路径在重写列表里)PS：可用于控制Task脚本
安装方法
安装路径教程：https://docs.boxjs.app或https://github.com/chavyleung/boxjs-doc或https://github.com/chavyleung/scripts
# 安装路径: 
 ​ 风车 > 重写 > 引用
# 重写路径: 
https://raw.githubusercontent.com/chavyleung/scripts/master/box/rewrite/boxjs.rewrite.quanx.conf
用法
浏览器访问：http://boxjs.com
boxjs技巧：https://docs.boxjs.app/base/tips
主屏幕添加：safari点中间小箭头→主屏幕添加
大佬电报：https://t.me/chavyscripts
大佬chavyleung仓库：https://github.com/chavyleung


表头|表头
--|--
内容|内容
; 更新时间2022-05-13 建建哥阿
; 哔哩哔哩和爱奇艺策略组用法
; 哔哩哔哩如要看港澳台剧，配置好规则前提下，切换对应节点即可
; 爱奇艺要看港澳台剧，配置好规则前提下，需应用里切换地区后，再去切换节点

# 规则类型优先级
在 Quantumult X 中并不是完全按顺序匹配，各类型的优先级应该为： host > host-suffix > host-keyword > user-agnet > geoip & ip-cidr。

# 相信看了前面大佬们的教程已经对Quanmutult X有更深入的了解，可以自己去配置，不需再用小白配置
## 以下是个人对配置路径的理解
# general模块内为一些通用的设置参数项
# [general]
## QuantumultX会对server_check_url指定的网址进行相应测试，以确认节点的可用性(默认的也可修改)
server_check_url=http://www.qualcomm.cn/generate_204
## 配置文件路径显示头像(不清楚在哪显示)
profile_img_url=https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/img/dragonball/1.PNG
## 下列表中内容将不经过QuantumultX的处理(默认的)
excluded_routes=10.0.0.0/8, 127.0.0.0/8, 169.254.0.0/16, 192.0.2.0/24, 192.168.0.0/16, 198.51.100.0/24, 224.0.0.0/4
# list中的域名将不使用fake-ip方式, 多个域名用“, ”连接。其它域名则全部采用 fake-ip及远程解析的模式
dns_exclusion_list = *.cmpassport.com, *.jegotrip.com.cn, *.icitymobile.mobi, id6.me, *.pingan.com.cn, *.cmbchina.com, *.localnetwork.uop, mfs.ykimg.com*.ttf, *.icbc.com.cn
# IP_bili_cn js-用于获取、展示节点信息，可完整自定义
geo_location_checker=http://api.live.bilibili.com/ip_service/v1/ip_service/get_ip_addr? , https://cdn.jsdelivr.net/gh/KOP-XIAO/QuantumultX@master/Scripts/IP_bili_cn.js
# 备用geo_location_checker=http://ip-api.com/json/?lang=zh-CN, https://raw.githubusercontent.com/Orz-3/Orz-3/master/QuantumultX/IP.js
# 资源解析器，自定义各类远程资源的转换、如节点、规则、filter、复写、rewrite等
resource_parser_url=https://cdn.jsdelivr.net/gh/KOP-XIAO/QuantumultX@master/Scripts/resource-parser.js
