# Google-Cloud

谷歌VM实例系统里面 没有Debian8了

所以大家改用CentOS6 （就没蓝底那个窗口了）

也可以使用debian9(推荐）
使用debian9 可以只用从第5步开始（当然sudo -i 这一步还是要的）只需2步就可以搭建好。不用装BBR加速器 速度也非常的快 直接破百兆！
1：sudo -i

(最前面显示root@xxxx)

2：wget -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/YankeeBBR/master/bbr.sh && bash bbr.sh install

蓝底窗口按TAB键选NO

选择重启 Y

这里会断开连接，大家可以关掉窗口再重新打开或几秒钟后在界面随便按几个字母 便会提示重新连接。

3：sudo -i

(最前面显示root@xxxx)

4：bash bbr.sh start

5：wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh && chmod +x shadowsocksR.sh

6：./shadowsocksR.sh

输入shadowsocks 密码

输入端口号

其他一路回车（也可自行选择混淆 协议）

在最后出现红底数据以后

谷歌云防火墙规则添加 （位置在谷歌云 VPC网络-防火墙）
点击添加新规则，然后按照一下这个设置好。这样 SSR 设置任何端口都可以使用。并且后续不需要再来防火墙规则做设置了。

