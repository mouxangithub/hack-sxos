# 破解版免费的SXOS License证书和个性化SXOS主题和多引导生成器

## 下载地址 => [hacksxos.exe](https://gitee.com/mouxangitee/hack-sxos/releases)

## 说明
源py脚本出自外网 [ **Hack SXOS License By Reacher17** ](https://gbatemp.net/threads/hack-sxos.582831/page-63) 本人只是对脚本做了一些简单的封装及加入了中文提示，并未修改其底层；该版本为截止至2021.07.01最新的版本，可重启不会提示boot丢失，及一些SX的程序Tinfoil，金手指等亦可用，具体自行测试
另外，软破真实系统最新目前12.0.3还能继续玩TX的11.0.0的虚拟系统，但硬破不行，硬破你只要真实升到12.0.2以上就彻底完犊子进不去了，哪怕降级也不行，除非tx更新，但软破没事，具体可了解下paulzheng.大佬发布的 [ **【闲聊】Mariko机型为什么没必要降级真实系统** ](https://www.91wii.com/thread-251267-1-1.html)

## 重点说明
### 硬破机无法使用，如果你是硬破机可了解下，但目前暂时没法用于硬破机 

## 使用教程
1. 因已经打包成了exe文件，无需另外安装py环境，可直接运行，如用py脚本运行者自行安装环境和依赖包
2. 运行hacksxos.exe脚本文件，脚本内置3.1的boot.dat已更名boot_ori.dat下载（首次如若无则默认下载，之后无需下载），亦可自行下载最新的更名
3. 第二个选项：是否设置开机跳过boot: 是 (y): 否 (n)，即：是否直接跳过boot，如果选是则之后哪怕开机+音量加都无法进入boot，所以建议关闭，默认关闭
4. 第三选项中脚本内置主题文件源自外网 [ **Custom SXOS CFW** ](https://gbatemp.net/threads/custom-sxos-cfw.588020/#post-9463428)，如需自定义请将修改好的主题文件放置themes文件夹，然后重新运行脚本，格式需为bmp，脚本会自动运行GFX_sxos.exe文件(将图片转换成bin文件再写入，这是[ **Reacher17** ](https://gbatemp.net/threads/hack-sxos.582831/page-63)大佬写的脚本就需要这样写入图片),具体自行研究
5. 第四选项：是否新增一个引导: 是 (y): 否 (n)，即：新增第四个引导按钮，然后下一项需输入新增的按钮引导的RCM文件(.bin结尾)，引导至大气层为：atmosphere/fusee-secondary.bin，默认引导的是hekate的payload.bin(可下载hekate的bin引导或者其他的)，然后设置button下方的引导按钮的名称
6. 关于免费的license证书，在 [ **Reacher17** ](https://gbatemp.net/threads/hack-sxos.582831/page-63) 的文章中，获取免费的license证书的方法有三种：
- fingerprint.txt + 脚本 +boot.dat 生成的是欺骗的boot.dat则不需要license证书（不知道这意思对不对，可以看这条 jonoxley大佬评论的，这种本人未测试过）
- 脚本 +boot.dat  生成的是 boot.dat + 通用欺骗license证书（本篇下方下载链接有打包的四按钮引导和原版三引导的）
- license-request.dat + 脚本 + boot.dat 生成的是破解版假license证书
按照大佬的意思是：前面两个是欺骗boot.dat的证书，而且最后一个是破解的假的license证书，欺骗的证书意味着真正的证书，具体我也不太清楚，应该三者没有太大的区别

为了照顾一些不会捣鼓python的朋友，所以下方我打包生成了一个有四引导按钮的和原版三引导的通用版license证书默认SXOS原版主题，如需自定义主题请下脚本进行编译打包转换，此处就不放置太多了，另外已打包exe可直接运行脚本，可无需python环境内置了