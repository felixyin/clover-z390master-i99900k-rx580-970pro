# clover-z390master-i99900k-rx580-970pro

黑苹果efi，适配技嘉z390系列、i99900k、rx580、970pro等硬件


# 适配硬件
- 主板：理论适配z390系列主板，技嘉兼容更好
- cpu：i9 9900k、ks、f
- 显卡：rx580 满血版，理论上rx开头可以黑苹果的A卡在efi上无区别
- m2固态：理论上可以安装黑苹果的固态，efi驱动无区别，详情百度可以黑苹果的硬件
- 内存：品牌随便，建议16g以上

# 注意事项
1. 禁用主板m2口：

clover-z390master-i99900k-rx580-970pro/EFI/CLOVER/ACPI/patched/目录下的：
- SSDT-RMWindows10.aml，是在efi启动macosx的时候禁止加载z390 master第二个ssd，我安装了windows的盘。
- SSDT-RMJinTaiKe1T.aml，是因为金泰克的ssd会导致无法进入黑苹果，因接到了第三个口，所以禁用主板上的第三个m2接口。

建议网友使用efi前，将以上2文件删除，如有需要后期可以增加。
> 在macos中禁用某些硬件的原因是可能采购了不兼容黑苹果的硬件（笔者本来是采购金泰克1tssd用作timemachine，但发现不兼容），但是windows下可能要使用这些硬件。

2. 技嘉主板原装网卡冲突问题解决办法：
   
   1)：拆解主板，去掉自带网卡

   2)：咨询技嘉售后，看bios中是否提供开关兼用网卡，或者升级bios后找一下

> 以上办法二选一，建议直接上螺丝刀去掉原装网卡。

3. macos安装前，尽量移除上面没有列出的硬件和外置usb设备，保持干净，先能够安装进入macos就是成功的一大步。

4. 技嘉主板安装黑苹果前，需进入bios进行设置，具体设置事项请百度或加黑苹果群询问。

# 其他

1. 安装macos后，可能需要一些辅助软件进行进一步的自定义，具体软件请QQ加“黑屏果”群，群文件里一般有。
2. 睡眠、handxx接力、投屏、声卡、蓝牙、无线（硬件请淘宝黑苹果网卡 博通4天线）、双4k显示器等，驱动完美。
3. 如果有需要连接外置雷电三设备，建议入手z390 设计师主板，自带两个雷电三接口，可省掉后期添加转接卡的钱。


# 必看截图



![](https://raw.githubusercontent.com/felixyin/clover-z390master-i99900k-rx580-970pro/master/screenshots/1.jpg)

![](https://raw.githubusercontent.com/felixyin/clover-z390master-i99900k-rx580-970pro/master/screenshots/2.jpg)

![](https://raw.githubusercontent.com/felixyin/clover-z390master-i99900k-rx580-970pro/master/screenshots/3.jpg)
> 此处有口误，改为：完美睡眠，不存在常见的各种睡眠问题。

![](https://raw.githubusercontent.com/felixyin/clover-z390master-i99900k-rx580-970pro/master/screenshots/4.jpg)

![](https://raw.githubusercontent.com/felixyin/clover-z390master-i99900k-rx580-970pro/master/screenshots/5.jpg)

![](https://raw.githubusercontent.com/felixyin/clover-z390master-i99900k-rx580-970pro/master/screenshots/6.jpg)


如上面图片无法查看，可以点击下面地址：

https://tva1.sinaimg.cn/large/006tNbRwly1g9q5o0mwonj310y0lwqhj.jpg

https://tva1.sinaimg.cn/large/006tNbRwly1g9q5pvzqhcj31yo0u04qq.jpg

https://tva1.sinaimg.cn/large/006tNbRwly1g9q5rd9cadj31140ou423.jpg

https://tva1.sinaimg.cn/large/006tNbRwly1g9q5szqmswj31zu0u0hdt.jpg

https://tva1.sinaimg.cn/large/006tNbRwly1g9q5yyqvvnj32q40u0kjn.jpg

https://tva1.sinaimg.cn/large/006tNbRwly1g9q6js5y3aj31460u0b2a.jpg