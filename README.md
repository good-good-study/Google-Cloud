# Google-Cloud

谷歌VM实例系统里面 ，选择使用debian9

1: sudo -i

(最前面显示root@xxxx)

2: bash <(curl -s -L https://git.io/v2ray.sh)

剩下的按提示输入一路畅通...

其他一路回车（也可自行选择混淆 协议）

在最后出现红底数据以后，就可以通过shadow工具使用啦

谷歌云防火墙规则添加 （位置在谷歌云 VPC网络-防火墙）
点击添加新规则，然后按照一下这个设置好。这样 SSR 设置任何端口都可以使用。并且后续不需要再来防火墙规则做设置了。

![image](https://github.com/good-good-study/Google-Cloud/blob/master/%E9%98%B2%E7%81%AB%E5%A2%99%E8%A7%84%E5%88%99%E9%85%8D%E7%BD%AE.png)

在配置完shadow工具后，来测试下我们的翻墙网速，Google Play Store 下载应用的速度还是相当可以的

![image](https://github.com/good-good-study/Google-Cloud/blob/master/vpn.gif)

