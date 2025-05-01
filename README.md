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


dns:  
  enable: true   
  ipv6: false 
  default-nameserver: [223.5.5.5,119.29.29.29,114.114.114.114］  
  
  enhanced-mode: fake-ip   
  fake-ip-range: 198.18.0.1/16  
  use-hosts: true   
  respect-rules: true   
  proxy-server-nameserver: ［223.5.5.5,119.29.29.29,114.114.114.114]
  nameserver: ['https://doh.pub/dns-query', 'https://dns.alidns.com/dns-query']
  fallback: ['https://doh.dns.sb/dns-query', 'https://dns.cloudflare.com/dns-query', 'https://dns. twnic. tw/dns-query','tls://8.8.4.4:853']  
  fallback-filter: { geoip: true, geoip-code: CN, geosite: [gfw], ipcidr:[240.0.0.0/4], domain: [+.google.com, +. facebook.com,+.youtube.com }  
  
