QuantumultX
自用规则，不定期更新，不建议引用，有需要自行复制。

# 介绍
## Bilibili.qxrewrite
**修改自blackmatrix7、app2smile两位大佬的规则，与原规则相比差异如下：**  
1、使用app2smile大佬proto脚本，有效去除播放界面up主推荐广告等顽固广告。  
2、调整blackmatrix7大佬部分规则。  
3、极限精简b站界面。  

## Quan_ADJS.conf
**自用去广告规则**  
京东极限精简首页以及个人页，删除无用推荐  
飞客茶馆去处广告   
米家去除广告并精简场景页面  
什么值得买引用于blackmatrix7大佬  

## Zhihu_Modified.qxrewrite
**此版本用reject屏蔽sugar.zhihu.com的请求，避免了之前各位大佬版本知乎频繁发送log的情况。**  
适用于7.30以上版本的知乎，请在filter_local添加如下内容  
[filter_local]  
#知乎去广告，以下规则请放置在filter_local最顶部  
IP-CIDR,118.89.204.198/32,REJECT  
IP6-CIDR,2402:4e00:1200:ed00:0:9089:6dac:96b6/128,REJECT  
HOST,118.89.204.198,REJECT  
#知乎去广告，以下规则的位置越前方越好  
HOST,appcloud2.in.zhihu.com,REJECT  
HOST,mqtt.zhihu.com,reject  
USER-AGENT,AVOS*,REJECT  

## Zhihu_lite.qxrewrite
**此版本用reject屏蔽sugar.zhihu.com的请求，避免了之前各位大佬版本知乎频繁发送log的情况。**  
适用于7.27以下版本的知乎，请在filter_local添加如下内容  
[filter_local]  
#知乎去广告，以下规则请放置在filter_local最顶部  
IP-CIDR,118.89.204.198/32,REJECT  
IP6-CIDR,2402:4e00:1200:ed00:0:9089:6dac:96b6/128,REJECT  
HOST,118.89.204.198,REJECT  
#知乎去广告，以下规则的位置越前方越好  
HOST,appcloud2.in.zhihu.com,REJECT  
HOST,mqtt.zhihu.com,reject  
USER-AGENT,AVOS*,REJECT  
