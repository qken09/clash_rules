# clash_rules
clash rules


规则：  
  
举例：  
https://raw.githubusercontent.com/qken09/clash_rules/refs/heads/main/proxy.txt
https://raw.githubusercontent.com/qken09/clash_rules/refs/heads/main/direct.txt
https://raw.githubusercontent.com/qken09/clash_rules/refs/heads/main/apple.txt
https://raw.githubusercontent.com/qken09/clash_rules/refs/heads/main/icloud.txt
https://raw.githubusercontent.com/qken09/clash_rules/refs/heads/main/china_ip_list.txt
https://raw.githubusercontent.com/qken09/clash_rules/refs/heads/main/AntiAD_com.txt
https://raw.githubusercontent.com/qken09/clash_rules/refs/heads/main/AntiAD_ip_list.txt
  
或  
https://raw.githubusercontent.com/qken09/clash_rules/16218ff1a20e03baca2f0b60b91e82738fad5a87/proxy.txt
https://raw.githubusercontent.com/qken09/clash_rules/16218ff1a20e03baca2f0b60b91e82738fad5a87/direct.txt
https://raw.githubusercontent.com/qken09/clash_rules/16218ff1a20e03baca2f0b60b91e82738fad5a87/apple.txt
https://raw.githubusercontent.com/qken09/clash_rules/16218ff1a20e03baca2f0b60b91e82738fad5a87/icloud.txt
https://raw.githubusercontent.com/qken09/clash_rules/16218ff1a20e03baca2f0b60b91e82738fad5a87/china_ip_list.txt
https://raw.githubusercontent.com/qken09/clash_rules/16218ff1a20e03baca2f0b60b91e82738fad5a87/AntiAD_com.txt
https://raw.githubusercontent.com/qken09/clash_rules/16218ff1a20e03baca2f0b60b91e82738fad5a87/AntiAD_ip_list.txt
  
参考出处：  
https://fastly.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/  
https://fastly.jsdelivr.net/gh/17mon/china_ip_list@master/  
https://whatshub.top/rule/  

  
图标：  
  
举例：  
https://raw.githubusercontent.com/qken09/clash_rules/refs/heads/main/png/Taiwan.png    
https://raw.githubusercontent.com/qken09/clash_rules/80e07f308440264df87ec3b364429cad8b8ad527/png/Taiwan.png
  
参考出处：  
https://fastly.jsdelivr.net/gh/Koolson/Qure@latest/IconSet/Color/  
https://fastly.jsdelivr.net/gh/Koolson/Qure@master/IconSet/Color/

数据库：  
GeoIP数据库：  https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/geoip-lite.dat  
GeoSite数据库：  https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/geosite.dat  
MMDB数据库：  https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/geoip.metadb  
ASN数据库：  https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/GeoLite2-ASN.mmdb  

dns:
  enable: true
  ipv6: false
  listen: ':53'
  enhanced-mode: 'fake-ip'
  fake-ip-range: '198.18.0.1/16'
  fake-ip-filter-mode: 'blacklist'
  prefer-h3: false
  respect-rules: true
  use-hosts: true
  use-system-hosts: true
  fake-ip-filter:
    - '*.lan'
    - '*.local'
    - '*.arpa'
    - time.*.com
    - ntp.*.com
    - time.*.com
    - +.market.xiaomi.com
    - localhost.ptlogin2.qq.com
    - '*.msftncsi.com'
    - www.msftconnecttest.com
    - localhost.ptlogin2.qq.com
    - localhost.sec.qq.com
    - localhost.work.weixin.qq.com
  default-nameserver:
    - 223.5.5.5
    - 119.29.29.29
    - 94.140.14.14
    - system
  nameserver:
    - https://doh.pub/dns-query
    - https://dns.alidns.com/dns-query
  direct-nameserver-follow-policy: false
  fallback:
    - 'https://doh.dns.sb/dns-query'
    - 'https://dns.cloudflare.com/dns-query'
    - 'https://dns.twnic.tw/dns-query'
    - 'tls://8.8.4.4:853'
  fallback-filter:
    geoip: true
    geoip-code: 'CN'
    geosite: 
      - gfw
    ipcidr:
      - '240.0.0.0/4'
      - '0.0.0.0/32'
    domain:
      - '+.google.com'
      - '+.facebook.com'
      - '+.youtube.com'
  proxy-server-nameserver:
    - 'https://223.5.5.5/dns-query'
    - 'https://doh.pub/dns-query'
  follow-rule: null
  skip-cert-verify: true

