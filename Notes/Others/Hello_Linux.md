## linux翻墙

1. 浏览器安装`SwitchyOmega`插件，设置代理为本地 `127.0.0.1 socks5`

2. 下载`shadowsock qt5`  按照ss的设置方法设置


## linux中安装node（不能全局翻墙的状态下）
> github.com/creationix/nvm

1. 根据文档安装完成后，重启终端（重要！）
2. 使用nvm install node 进行安装

## linux 快捷键

- `ALT + F1`: 聚焦到桌面左侧任务导航栏，可按上下键导航。
- `CTRL + ALT + T`: 打开终端
- `TAB`: 自动补全命令或文件名
- `CTRL + SHIFT + V`: 粘贴（Linux中不需要复制的动作，文本被选择就自动被复制）
- `CTRL + SHIFT + T`: 新建标签页
- `CTRL + D`: 关闭标签页
- `CTRL + L`: 清楚屏幕
- `CTRL + R` + 文本: 在输入历史中搜索
- `CTRL + A`: 移动到行首
- `CTRL + E`: 移动到行末
- `CTRL + C`: 终止当前任务
- `CTRL + Z`: 把当前任务放到后台运行（相当于运行命令时后面加&）

## Linux下挂载exfat盘

```
sudo su  
add-apt-repository ppa:relan/exfat  
apt-get update  
apt-get install exfat-utils  
```

## Ubuntu 14.04下安装Qt5

`sudo apt-get update` 
`sudo apt-get install libqt4-dev libqtwebkit-dev`
`sudo apt-get install qt5-default libqt5webkit5-dev gstreamer1.0-plugins-base gstreamer1.0-tools gstreamer1.0-x`

如果qmake还是找不到，需要在环境变量里把qmake和最新版本的qt里的qmake关联起来

```
which qmake # to see where it links
rm `which qmake` # IF it is linking to an old version 
```

## linux修改文件权限

sudo chmod -R 777 files/
