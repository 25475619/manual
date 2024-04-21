#==========================================
#@configName 墨鱼自用Surfboard配置文件
#@Author@ddgksf2013
#@TgChannel 𝐡𝐭𝐭𝐩𝐬://𝐭.𝐦𝐞/𝐝𝐝𝐠𝐤𝐬𝐟𝟐𝟎𝟐𝟏
#@微信ID公众号@墨鱼手记
#@Feedback           💡请通过邮件反馈问题[其它方式一概无视]：𝐝𝐝𝐠𝐤𝐬𝐟𝟐𝟎𝟏𝟑@𝟏𝟔𝟑.𝐜𝐨𝐦  💡
#@UpdateTime2024/04/1922:35UTC/GMT+8
#@函数支持手动选择、自动测速、广告屏蔽、兜底分流、按国家分组节点、多机场订阅等
#@Thanks@blackmatrix7，@猫队，@DivineEngine
#@Attention          𝐏𝐥𝐞𝐚𝐬𝐞 𝐠𝐨 𝐭𝐨 𝐆𝐨𝐨𝐠𝐥𝐞 𝐏𝐥𝐚𝐲 𝐒𝐭𝐨𝐫𝐞 𝐭𝐨 𝐝𝐨𝐰𝐧𝐥𝐨𝐚𝐝 𝐭𝐡𝐞 𝐥𝐚𝐭𝐞𝐬𝐭 𝐒𝐮𝐫𝐟𝐛𝐨𝐚𝐫𝐝
#@ConfigVersion1.0.3
#==========================================

[一般的]

loglevel=notify
interface=127.0.0.1
skip-proxy=127.0.0.1，192.168.0.0/16,10.0.0.0/8，172.16.0.0/12，100.64.0.0/10，localhost，*.local
IPv6=false
dns-server=系统，223.5.5.5
exclude-simple-hostname=true
按规则增强模式=true

[代理]


[代理组]

🚀 手动切换=select， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，direct，policy-path=https://api.nexconvert.com/sub?target=surfboard&url=请手动填写你的机场订阅&insert=false&emoji=false&list=true&tfo=false&scv=false&fdn=false&sort=false，间隔=300，更新间隔=86400

#分流分组
🌏 国外网站=select， 🚀 手动切换， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，直接，无警报=0，隐藏=0
📽️ 国际媒体=select， 🚀 手动切换， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，直接，无警报=0，隐藏=0
🖥️ 微软服务=select， 🚀 手动切换， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，直接，无警报=0，隐藏=0
🌌 谷歌服务=select， 🚀 手动切换， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，直接，无警报=0，隐藏=0
📟 电报消息=select， 🚀 手动切换， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，直接，无警报=0，隐藏=0
🐦 推特消息=select， 🚀 手动切换， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，直接，无警报=0，隐藏=0
🤖  OpenAI=select， 🚀 手动切换， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，直接，无警报=0，隐藏=0
📺 哔哩哔哩=select，DIRECT， 🇭🇰 香港节点， 🇨🇳 台湾节点，no-alert=0，hidden=0
🛑 广告拦截=选择、拒绝、直接、无警报=0、隐藏=0
🐟 兜底分流=select， 🚀 手动切换， 🇭🇰 香港节点， 🇺🇸 美国节点， 🇸🇬 狮城节点， 🇯🇵 日本节点， 🇨🇳 台湾节点，no-alert=0，hidden=0

# 自动测速
🇭🇰 香港节点=url-test，policy-regex-filter=港|HK|(？I)Hong，interval=600，update-interval=86400，no-alert=0，hidden=0，include-other-group="🚀 手动切换"
🇯🇵 日本节点=url-test，policy-regex-filter=日|东京|JP|(？I)日本，interval=600，update-interval=86400，no-alert=0，hidden=0，include-other-group="🚀 手动切换"
🇨🇳 台湾节点=url-test，policy-regex-filter=台|湾|TW|(？I)台湾，interval=600，update-interval=86400，no-alert=0，hidden=0，include-other-group="🚀 手动切换"
🇺🇸 美国节点=url-test，policy-regex-filter=美|US|(？I)状态|美国，时间间隔=600，更新时间间隔=86400，无警报=0，隐藏=0，include-other-group="🚀 手动切换"
🇸🇬 狮城节点 = url-test, policy-regex-filter=新|坡|SG|(?i)Singapore, interval=600, update-interval=86400, no-alert=0, hidden=0, include-other-group = "🚀 手动切换"

[Rule]

# 分流规则 
RULE-SET,https://cdn.jsdelivr.net/gh/Cats-Team/AdRules@main/adrules.list,🛑 广告拦截
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/OpenAI/OpenAI.yaml,🤖 OpenAi
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Telegram/Telegram.yaml,📟 电报消息
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Twitter/Twitter.yaml,🐦 推特消息
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/GitHub/GitHub.yaml,🖥️ 微软服务
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/OneDrive/OneDrive.yaml,🖥️ 微软服务
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Microsoft/Microsoft.yaml,🖥️ 微软服务
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/YouTube/YouTube.yaml,🌌 谷歌服务
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Google/Google.yaml,🌌 谷歌服务
RULE-SET,https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/BiliBili/BiliBili.yaml,📺 哔哩哔哩
RULE-SET,https://cdn.jsdelivr.net/gh/ddgksf2013/Filter@master/Streaming.list,📽️ 国际媒体
RULE-SET,https://cdn.jsdelivr.net/gh/DivineEngine/Profiles@master/Surge/Ruleset/Global.list,🌏 国外网站
GEOIP,CN,DIRECT
最终的，🐟 兜底分流
