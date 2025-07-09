这里是红米ax6000-128M-U-boot固件，基于immortalwrt-24.10，自带adguardhome,passwall,uugamebooster,alist，可修改代码增加自己需要的插件，直接fork即可云编译，毫无保留。
  
地址为192.168.6.1 需要修改的自行在diy-part2.sh文件第二十行里修改
action后，在SSH connection to Actions连接选项输入true,
run workflow
等待出现SSH链接，并点击打开新页面
进入ssh连接页面后
ctrl+c
输入 cd openwrt && make menuconfig 进入图形选择界面，选择好所需插件后保存退出。LuCI ---> Applications 选择所需的插件

退出后输入ctrl+D
ACTION会自动开始后面的操作
