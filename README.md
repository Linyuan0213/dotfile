# i3wm配置

**Screenshot**

![Screenshot](https://github.com/Linyuan0213/dotfile/blob/master/SCREENSHOT.png?raw=true)

### i3需要安装软件 

- *i3-wm*

- *i3gaps*

- *feh* 设置背景图片

- *mpd  ncmpcpp*播放音乐

- *urxvt* 终端

- *polybar* 状态栏

- *compton* 终端透明

- *i3lock-fancy-git* 锁屏

- *ranger* 浏览文件

- *roli* 程序启动和窗口切换

### 安装

  #### 1. 字体安装


  ```
  aurman -S ttf-font-awesome
  ```

  #### 2. 安装软件

  ```
  aurman -S rxvt-unicode feh compton i3-gaps i3lock-fancy-git  polybar-git ranger mpd ncmpcpp
  ```

  

  ### 使用

  ####  启动 i3

  有多种启动方式，这里使用 `startx` 命令的方式。先添加下面一行文字到`.xinitrc`文件中：

  ```
  exec i3
  ```

  如果想记录 i3 所有的输日志，添加：

  ```
  exec i3 -V >> ~/i3log-$(date +'%F-%k-%M-%S') 2>&1
  ```

  添加完了之后，执行 `startx` 启动 i3 。

  

###  配置

​	下载本配置文件并解压，将i3wm 文件夹下的i3、mpd和polybar复制到~/.config下；

urxvt目录下的.Xresources复制到 **~/** 下，执行xrdb -merge  $HOME/.Xresources生效

 如果使用startx启动可以将xrdb -merge  $HOME/.Xresources加到.xinitrc中

