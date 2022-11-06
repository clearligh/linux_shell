
<div align=center>
<img src="https://docs.espressif.com/projects/esp-idf/zh_CN/v4.3/esp32c3/_images/linux-logo.png" width="150" height="150">
</div>

#  <center> Linux一键脚本汇总
## *Scoks5 一键搭建脚本* 

### <center> 系统支持：  
        CentOS 6.x    
        CentOS 7.x  
### 介绍  
一个 Shell 脚本，集成 Socks5 搭建，管理，启动，添加账号等基本操作。基于 Socks5 官方的辅助脚本，方便用户操作，并且支持快速构建 Socks5 服务环境。  
### 代码  
```
wget -q -N --no-check-certificate https://raw.githubusercontent.com/wyx176/Socks5/master/install.sh && bash install.sh
```
### 功能  
* 一键开启、关闭 ss5 服务
* 添加账户，删除用户，开启账户验证，关闭账户验证，一键修改端口
* 支持傻瓜式用户添加，小白也可以用
* 自动修改防火墙规则
* 输入 s5 即可启动控制面板

## *一键安装宝塔纯净版 7.6.0版本[宝塔纯净版](https://www.hostcli.com/ "宝塔纯净版")*
Centos全新安装命令  
```
yum install -y wget && wget -O install.sh http://v7.hostcli.com/install/install_6.0.sh && sh install.sh
```
Debian全新安装命令
```
wget -O install.sh http://v7.hostcli.com/install/install-ubuntu_6.0.sh && bash install.sh
```
Ubuntu/Deepin全新安装命令
```
wget -O install.sh http://v7.hostcli.com/install/install-ubuntu_6.0.sh && sudo bash install.sh
```

## *一键安装BBR加速脚本*
```
wget -N --no-check-certificate "https://gist.github.com/zeruns/a0ec603f20d1b86de6a774a8ba27588f/raw/4f9957ae23f5efb2bb7c57a198ae2cffebfb1c56/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
```
### 功能  
* 一键开启、关闭 BBR、BBRPLUS、BBR魔改，锐速(Lotsever) 服务
* 支持傻瓜式用户添加，小白也可以用
* 支持一键系统配置优化

## *NaïveProxy一键搭建脚本*
安装 naive命令
```
curl   https://raw.githubusercontent.com/imajeason/nas_tools/main/NaiveProxy/do.sh | bash
```
执行naive一键脚本
```
naive
```
### 功能  
* 一键开启、关闭 naiveproxy 服务
* 添加账户，删除用户，开启账户验证，关闭账户验证，一键修改端口
* 支持傻瓜式用户添加，小白也可以用
* 自动修改防火墙规则
* 输入 naive 即可启动控制面板
### 优化命令
添加定时任务，更新证书
```
touch /var/spool/cron/root
echo "0 1 * * * /etc/caddy/.renew.sh" >> /var/spool/cron/root
ls /etc/caddy/.renew.sh
#查询是否设置成功
/etc/caddy/.renew.sh
```
重启Naive（由于目前naive运行久了会降速，所以还是建议经常重启）
```
systemctl restart naive
```

## *一键搭建hysteria服务端*
```
wget https://raw.githubusercontent.com/lanhebe/hysteria/master/onekey_installHysteria.sh && chmod +x onekey_installHysteria.sh && ./onekey_installHysteria.sh
```
### 功能  
* 一键安装、卸载 hysteria 服务端

## *一键安装Telegram代理脚本（伪装）*
```
wget -N --no-check-certificate https://github.com/whunt1/onekeymakemtg/raw/master/mtproxy_go.sh && chmod +x mtproxy_go.sh && bash mtproxy_go.sh
```
### 功能  
* 一键设置端口
* 一键生成代理链接

## *一键安装swap的脚本*
```
wget -O box.sh https://raw.githubusercontent.com/BlueSkyXN/SKY-BOX/main/box.sh && chmod +x box.sh && clear && ./box.sh
```

## *流媒体解锁测试脚本*
```
bash <(curl -L -s https://raw.githubusercontent.com/lmc999/RegionRestrictionCheck/main/check.sh)
```
### 支持检测的流媒体
<div align="center">

| Netflix  | YouTube Premium| Amazon Prime Video| Spotify |
| ---------- | -----------| -----------| -----------|
| AQiYi OverSea  | Dazn | Disney+ | HotStar |
| BiliBili海外 | Viu.com | HBO GO Aisa | MyTvSuper |

</div>

## *三网回程延迟测试脚本*
```
wget -qO- git.io/besttrace | bash
```

## *三网回程测试脚本*
```
curl https://raw.githubusercontent.com/zhucaidan/mtr_trace/main/mtr_trace.sh|bash
```

## *三网测速脚本*
```
bash <(curl -Lso- https://git.io/superspeed_uxh)
```

## *整合测速命令*
```
wget -qO- --no-check-certificate https://raw.githubusercontent.com/oooldking/script/master/superbench.sh | bash
```
