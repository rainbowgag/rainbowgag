[custom]
;解决DNS泄露，无分流群组
ruleset=🚀 节点选择,[]DOMAIN-SUFFIX,services.googleapis.cn
ruleset=🚀 节点选择,RULE-SET,Telegram,📲 电报消息
ruleset=🚀 节点选择,RULE-SET,OpenAi,💬 OpenAi
ruleset=🚀 节点选择,RULE-SET,YouTube,📹 油管视频
ruleset=🚀 节点选择,RULE-SET,Netflix,🎥 奈飞视频
ruleset=🚀 节点选择,RULE-SET,Bahamut,📺 巴哈姆特
ruleset=🚀 节点选择,[]DOMAIN-SUFFIX,xn--ngstr-lra8j.com
ruleset=🚀 节点选择,[]DOMAIN-SUFFIX,services.googleapis.cn
ruleset=🚀 节点选择,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/GoogleCNProxyIP.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/LocalAreaNetwork.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/UnBan.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaDomain.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaMedia.list
ruleset=REJECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanAD.list
ruleset=REJECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanProgramAD.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaCompanyIp.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaIp.list
ruleset=DIRECT,[]GEOIP,CN,no-resolve
ruleset=🚀 节点选择,[]FINAL

custom_proxy_group=🚀 节点选择`select`["🇭🇰 香港节点", "🇹🇼 台湾节点", "🇯🇵 日本节点", "🇸🇬 新加坡节点", "🇺🇸 美国节点", "🇰🇷 韩国节点"]♻️ 自动选择`[]DIRECT`.*
custom_proxy_group=♻️ 自动选择`url-test`.*`http://www.gstatic.com/generate_204`300,,50
custom_proxy_group=🎥 奈飞视频`select`["🇭🇰 香港节点", "🇹🇼 台湾节点", "🇯🇵 日本节点", "🇸🇬 新加坡节点", "🇺🇸 美国节点", "🇰🇷 韩国节点"]♻️ 自动选择`[]DIRECT`.*
custom_proxy_group=💬 OpenAi`select`["🇭🇰 香港节点", "🇹🇼 台湾节点", "🇯🇵 日本节点", "🇸🇬 新加坡节点", "🇺🇸 美国节点", "🇰🇷 韩国节点"]♻️ 自动选择`[]DIRECT`.*
custom_proxy_group=📲 电报消息`select`["🇭🇰 香港节点", "🇹🇼 台湾节点", "🇯🇵 日本节点", "🇸🇬 新加坡节点", "🇺🇸 美国节点", "🇰🇷 韩国节点"]♻️ 自动选择`[]DIRECT`.*
custom_proxy_group=📹 油管视频`select`["🇭🇰 香港节点", "🇹🇼 台湾节点", "🇯🇵 日本节点", "🇸🇬 新加坡节点", "🇺🇸 美国节点", "🇰🇷 韩国节点"]♻️ 自动选择`[]DIRECT`.*
custom_proxy_group=📺 巴哈姆特`select`["🇭🇰 香港节点", "🇹🇼 台湾节点", "🇯🇵 日本节点", "🇸🇬 新加坡节点", "🇺🇸 美国节点", "🇰🇷 韩国节点"]♻️ 自动选择`[]DIRECT`.*
custom_proxy_group=🇭🇰 香港节点`url-test`.*`http://www.gstatic.com/generate_204`300,,50.filter: (?i)香港|香江|Hong Kong|HK|🇭🇰|Hongkong
custom_proxy_group=🇹🇼 台湾节点,url-test.*http://www.gstatic.com/generate_204 300,,50.filter: (?i)台湾|TW|Taiwan|🇹🇼
custom_proxy_group=🇸🇬 新加坡节点,url-test.*http://www.gstatic.com/generate_204 300,,50.filter: (?i)新加坡|SG|Singapore|🇸🇬
custom_proxy_group=🇰🇷 韩国节点,url-test.*http://www.gstatic.com/generate_204 300,,50.filter: (?i)韩国|KR|South Korea|🇰🇷
custom_proxy_group=🇯🇵 日本节点,url-test.*http://www.gstatic.com/generate_204 300,,50.filter: (?i)日本|JP|Japan|🇯🇵|Tokyo

enable_rule_generator=true
overwrite_original_rules=true
