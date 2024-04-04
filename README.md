
<div align=center>
<img src="https://docs.espressif.com/projects/esp-idf/zh_CN/v4.3/esp32c3/_images/linux-logo.png" width="150" height="150">
</div>

# Linux一键脚本汇总


***



## 面板类搭建脚本

### 1. *宝塔面板开心版*

CentOS7安装命令

```
yum install -y wget && wget -O install.sh http://io.bt.sy/install/install_6.0.sh && sh install.sh
```

Ubuntu / Deepin安装命令

```
wget -O install.sh http://io.bt.sy/install/install-ubuntu_6.0.sh && sudo bash install.sh
```

Debian安装命令

```
wget -O install.sh http://io.bt.sy/install/install-ubuntu_6.0.sh && bash install.sh
```

### 2. *1Panel面板*

> 新一代的 Linux 服务器运维管理面板(主要是docker管理)

RedHat / CentOS安装命令

```
curl -sSL https://resource.fit2cloud.com/1panel/package/quick_start.sh -o quick_start.sh && sh quick_start.sh
```

Ubuntu安装命令

```
curl -sSL https://resource.fit2cloud.com/1panel/package/quick_start.sh -o quick_start.sh && sudo bash quick_start.sh
```

Debian安装命令

```
curl -sSL https://resource.fit2cloud.com/1panel/package/quick_start.sh -o quick_start.sh && bash quick_start.sh
```

### 3. *极光面板*

> 多服务器端口租用管理面板,可以添加多台服务器及端口，并将其分配给任意注册用户，租户则可以很方便地使用被分配的端口来完成各种操作，目前支持的端口功能
>
> - [iptables](https://www.netfilter.org/)
> - [socat](http://www.dest-unreach.org/socat/)
> - [gost](https://github.com/ginuerzh/gost)
> - [ehco](https://github.com/Ehco1996/ehco)
> - [realm](https://github.com/zephyrchien/realm)
> - [v2ray](https://github.com/v2fly/v2ray-core)
> - [brook](https://github.com/txthinking/brook)
> - [iperf](https://iperf.fr/)
> - [haproxy](http://www.haproxy.org/)
> - [wstunnel](https://github.com/erebe/wstunnel)
> - [shadowsocks](https://github.com/shadowsocks)
> - [tinyPortMapper](https://github.com/wangyu-/tinyPortMapper)
> - [Prometheus Node Exporter](https://github.com/leishi1313/node_exporter)
>
> 

安装脚本

```
bash <(curl -fsSL https://raw.githubusercontent.com/Aurora-Admin-Panel/deploy/main/install.sh)
# 国内机器安装可以选择使用 fastgit 镜像
# 但由于拉取 docker 镜像时候默认服务器仍在国外，可能拉取速度较慢
# 可自行搜索如何配置 Docker Hub 国内镜像加速
# bash <(curl -fsSL https://raw.fastgit.org/Aurora-Admin-Panel/deploy/main/install.sh) --mirror
```

### 4.  *X-ui面板*

> [支持多协议多用户的xray 面板](https://github.com/vaxilu/x-ui)
>
> 

安装命令

```
bash <(curl -Ls https://raw.githubusercontent.com/vaxilu/x-ui/master/install.sh)
```

### 5. *3X-ui面板*

安装与升级命令

```
bash <(curl -Ls https://raw.githubusercontent.com/mhsanaei/3x-ui/master/install.sh)
```

### 6. *哪吒面板*

> 开源、轻量、易用的服务器监控、运维工具

安装命令

```
curl -L https://raw.githubusercontent.com/naiba/nezha/master/script/install.sh  -o nezha.sh && chmod +x nezha.sh && sudo ./nezha.sh
```

大陆服务器可以使用镜像安装

```
curl -L https://gitee.com/naibahq/nezha/raw/master/script/install.sh -o nezha.sh && chmod +x nezha.sh && sudo CN=true ./nezha.sh
```

***



## 代理类搭建脚本

### 1. *BBR脚本*

>* 一键开启、关闭 BBR、BBRPLUS、BBR魔改，锐速(Lotsever) 服务
>* 支持傻瓜式用户添加，小白也可以用
>* 支持一键系统配置优化

```
wget http://sh.nekoneko.cloud/tools.sh -O tools.sh && bash tools.sh
```

### 2. *Hysteria2一键脚本*

```
wget -P /root -N --no-check-certificate "https://raw.githubusercontent.com/mack-a/v2ray-agent/master/install.sh" && chmod 700 /root/install.sh && /root/install.sh
```

### 3. *Scoks5 搭建脚本*

系统支持 : Centos 6.x 、Centos 7.x

> 一个 Shell 脚本，集成 Socks5 搭建，管理，启动，添加账号等基本操作。基于 Socks5 官方的辅助脚本，方便用户操作，并且支持快速构建 Socks5 服务环境。

安装命令

```
wget -q -N --no-check-certificate https://raw.githubusercontent.com/wyx176/Socks5/master/install.sh && bash install.sh
```

### 4. *MTProxy一键脚本*

> 可能是目前最方便的MTProxy脚本

安装命令

```
bash <(curl -sSL https://raw.githubusercontent.com/elesssss/MTProxy/main/mtproxy.sh)
```

### 5. *WARP 脚本*

安装命令

```
wget -N https://gitlab.com/fscarmen/warp/-/raw/main/menu.sh && bash menu.sh
```

或

```
wget -N https://gitlab.com/Misaka-blog/warp-script/-/raw/main/warp.sh && bash warp.sh
```

***



## 测试类脚本

### 1. *融合怪测试脚本*

> 功能介绍 :  [GitHub](https://github.com/spiritLHLS/ecs/blob/main/README.md#%E8%9E%8D%E5%90%88%E6%80%AA%E5%8A%9F%E8%83%BD)

安装命令

```
bash <(wget -qO- --no-check-certificate https://gitlab.com/spiritysdx/za/-/raw/main/ecs.sh)
```

### 3. *流媒体解锁测试脚本（支持原生）*

安装命令

```
bash <(curl -L -s media.ispvps.com)
```

***



## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=huajianyizou/linux_shell&type=Date)](https://star-history.com/#huajianyizou/linux_shell&Date)
