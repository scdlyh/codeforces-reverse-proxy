# codeforces-reverse-proxy
使用cloudflare的边缘计算服务workers反向代理指定网址
# 使用方法

1.在cloudflare里创建三个运行JavaScript的worker，分别把三个js文件作为源代码创建Workers服务分别代理不同的网址，网址1、网址2、网址3。
2.把cf.js里32行里的  'sta.cf.<YOUR-SUBDOMAIN>.workers.dev':'stacf.<YOUR-SUBDOMAIN>.workers.dev',    改为   '需要替换的网址':'步骤1可访问的Workers服务的网址1', 
3.把cf.js里33行里的  'sta.cf.<YOUR-SUBDOMAIN>.workers.dev':'stacf.<YOUR-SUBDOMAIN>.workers.dev',    改为   '需要替换的网址':'步骤1可访问的Workers服务的网址2', 
