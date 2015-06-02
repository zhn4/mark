#Ubuntu L2TP设置
###添加PPA
```
sudo apt-add-repository ppa:seriy-pr/network-manager-l2tp
```
###刷新软件包缓存
```
sudo apt-get update
```
###安装network-manager-l2tp
```
sudo apt-get install network-manager-l2tp-gnome
```
安装完后继续运行以下命令
```
sudo service xl2tpd stop 
sudo update-rc.d xl2tpd disable
```
最后重启一下机器，新建VPN的时候选择L2TP协议，其他配置跟PPTP一样