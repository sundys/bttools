宝塔降级7.7.0方法,这个版本可以不用强制登录宝塔账号

7.7.0安装方法:

纯原版安装：wget -O install.sh https://github.com/sundys/bttools/raw/master/install_6.0.sh && bash install.sh

如已经安装宝塔最新版降级脚本如下：

wget -O install.sh http://blog.fqidc.cn/bt/install_6.0.sh && bash install.sh

unzip LinuxPanel-*

cd panel

bash update.sh

cd .. && rm -f LinuxPanel-*.zip && rm -rf panel

备用降级下载地址：wget https://github.com/sundys/bttools/raw/master/LinuxPanel7.7.0/LinuxPanel-7.7.0.zip

执行以下脚本，解决强制登录宝塔账号提醒：

rm -f /www/server/panel/data/bind.pl

找到www/server/panel/data/这个目录并替换plugin目录下的两个文件

你就会发现付费软件全部可以免费用了

最后去面板设置里把宝塔离线模式打开，这样他就不会强制升级了

