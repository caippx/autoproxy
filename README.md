# autoproxy
更新一些简单修改自用的代理脚本，业余党，各种问题欢迎反馈-https://t.me/zqusb

## ssrjs.sh</br>
<b>ssr+tls+真实网站(jsproxy)</b></br>
该脚本参考教程-[ShadowsocksR服务端伪装成 正常网站流量，以更好的欺骗流量匹配](URL 'https://doubibackup.com/hi10k-7p-5.html') ，在逗比的脚本上屑改一波后制作而成。脚本安装的jsproxy运行在8443端口，并对主机ip进行免费的公共域名解析(xxx.xip.io)并申请SSL,该功能由JSproxy项目的一键脚本实现-https://github.com/EtherDream/jsproxy 。ShadowsocksR客户端将会运行在443端口，会将https网页请求转发到8443端口(jsproxy导航页)，实现jsproxy与ssr共存。</br>
<b>注意</b>：使用脚本安装时请确保80端口可以被外网访问，443和8443端口没有被占用！

<b>系统支持</b>: Debian 8+ x64</br>
真一键下载安装:</br>
```wget -N --no-check-certificate https://raw.githubusercontent.com/caippx/autoproxy/master/ssrjs.sh && chmod +x ssrjs.sh && bash ssrjs.sh auto```

真一键安装SSR默认使用该配置： </br>
```
端口:443
密码：ppxwo.com 
加密方式:chacha20-ietf 
协议：auth_aes128_md5
混淆：tls1.2_ticket_auth 
混淆参数：xxx.xip.io (xxx为你的主机ip)</p>
```
安装完成后，可通过 https://xxx.xip.io 访问你的jsproxy代理。(xxx为你的主机ip) </br>

管理命令:</br>
```
wget -N --no-check-certificate https://raw.githubusercontent.com/caippx/autoproxy/master/ssrjs.sh && chmod +x ssrjs.sh && bash ssrjs.sh
```
如有需要可以更改密码，其它参数不建议修改。
