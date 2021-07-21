# Unlock-netease-cloud-music

解锁网易云音乐客户端变灰歌曲

## 项目介绍

网易音乐相信不需要我过多的介绍大家也都知道，由于各种限制，相信很多人在听歌的时候也注意到了，很多的音乐呈现灰色的样式，是无法播放的，如下图所示。今天就带大家**把灰色不能听的音乐全部变成可以正常播放的音乐**，而且是**全平台通用**哦！

<span style="color:orangered;font-weight:bold;">注：教程有点长，如果实在没有耐心请直接滑到最下方观看浏览器听音乐方案</span>

[![g8Ogrd.png](https://z3.ax1x.com/2021/05/08/g8Ogrd.png)](https://imgtu.com/i/g8Ogrd)

## 特性

- 使用 QQ / 虾米 / 百度 / 酷狗 / 酷我 / 咪咕 / JOOX 音源替换变灰歌曲链接 (默认仅启用一、五、六)
- 为请求增加 `X-Real-IP` 参数解锁海外限制，支持指定网易云服务器 IP，支持设置上游 HTTP / HTTPS 代理
- 完整的流量代理功能 (HTTP / HTTPS)，可直接作为系统代理 (同时支持 PAC)

# <span style="color:orangered;font-weight:bold;">Windows端方法一：</span>

1.打开网易云音乐客户端，进入设置页面，设置自定义代理

- 自定义代理 ：填写服务器地址和端口号

- 代理服务器地址：127.0.0.1 

- 代理服务器端口：52000

  ![04GPKA.png](https://s1.ax1x.com/2020/10/14/04GPKA.png)

**2.安装node.js**

官方网站：[http://nodejs.cn/download/](http://nodejs.cn/download/)

下载后双击软件安装包打开安装，一直点下一步直到完成即可

![04G9vd.png](https://s1.ax1x.com/2020/10/14/04G9vd.png)

3.**下载项目源码**

**[https://github.com/meng-chuan/Unlock-netease-cloud-music/archive/refs/heads/master.zip](https://github.com/meng-chuan/Unlock-netease-cloud-music/archive/refs/heads/master.zip)**

下载后解压到任意文件夹,双击点开Unlock-netease-cloud-music文件夹中名为：网易☁🎵.bat 的文件

![04GpgH.png](https://s1.ax1x.com/2020/10/14/04GpgH.png)

注：此窗口不可关闭，可以最小化

以后每次打开网易云先运行网易☁🎵.bat这个文件即可解锁所有灰色歌曲，在这里先恭喜你成功学会了第一种解锁网易云音乐灰色歌曲的方法

# <span style="color:orangered;font-weight:bold;">Windows端方法二：</span>

注意：Windows 7 如无法执行则需升级 Powershell 到 3.0 以上，XP 不支持，**下载地址**：[https://docs.microsoft.com/powershell/scripting/install/installing-powershell](https://docs.microsoft.com/powershell/scripting/install/installing-powershell)

![04GiDI.png](https://s1.ax1x.com/2020/10/14/04GiDI.png)

**第一步，安装代理**

以 `管理员身份` 打开 `Powershell`，Windows 10 快捷入口：`Win + X` - `Windows Powershell(管理员)(A)`

![04GAVP.png](https://s1.ax1x.com/2020/10/14/04GAVP.png)

复制以下代码，右键粘贴到命令行回车，打开安装菜单。

```powershell
Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Force
Invoke-Expression -Command (Invoke-WebRequest -UseBasicParsing -Uri https://bit.ly/2RYvE3p).Content
```

![04GEUf.png](https://s1.ax1x.com/2020/10/14/04GEUf.png)

- 随后选择 `1` 即安装。
- 安装完毕后选择 `3` 运行。
- 如需添加开机自启，则执行 `7`。
- 最后输入 `0` 退出。

![04GV58.png](https://s1.ax1x.com/2020/10/14/04GV58.png)

**第二步，设置代理**

打开网易云音乐客户端，进入设置页面，设置自定义代理

- 自定义代理 ：填写服务器地址和端口号

- 代理服务器地址：127.0.0.1 （推荐本机搭建，速度快）

- 代理服务器端口：6666

  ![04GePS.png](https://s1.ax1x.com/2020/10/14/04GePS.png)

  如使用一段时间后无法解锁，则需要重新执行命令，选择 `5` 更新。

# <span style="color:orangered;font-weight:bold;">Windows端方法三：</span>

请移步最下方观看有服务器自己搭建方案

# <span style="color:orangered;font-weight:bold;">macOS端</span>

由于本人家境贫寒，买不起苹果电脑，又不想用黑苹果，无法截图说明，所以这里直接文字描述

请移步最下方观看有服务器自己搭建方案，搭建好后依次打开系统偏好`设置`＞`网络`＞`高级`＞`代理`，然后填入**地址**：ip地址+端口号/proxy.pac，例如：114.114.114.114:52000/proxy.pac

# <span style="color:orangered;font-weight:bold;">Linux端</span>

会用Linux的都不应该是小白，所以这里就不截图了，直接上文字描述

Linux端的使用也同样与以上macOS端方法同理，依次进入系统`设置`＞`网络`＞`网络代理`，然后填入**地址**：ip地址+端口号/proxy.pac，例如：114.114.114.114:52000/proxy.pac

#  <span style="color:orangered;font-weight:bold;">安卓端</span>

<span style="color:orangered;font-weight:bold;">**方法一：**</span>

安卓端是本人用了很久的一个小工具，这里先膜拜一下大佬的[开源项目](https://github.com/ndroi/easy163)，该软件无需**ROOT**，无需**WiFi**，一键解锁，接下来我用Redmi K30 Pro给大家演示一下

**第一步：进入浏览器输入地址https://github.com/ndroi/easy163/releases，选最新版本，下载后缀为apk的文件，然后安装**

![04DE9I.jpg](https://s1.ax1x.com/2020/10/14/04DE9I.jpg)

**第二步：打开软件，点击下面的按钮开启**

![04Dk4A.jpg](https://s1.ax1x.com/2020/10/14/04Dk4A.jpg)

**第三步：软件后台运行，进入网易云音乐你会发现所有音乐已经解锁成功了，下面放一张效果图**

[![g8zouD.png](https://z3.ax1x.com/2021/05/08/g8zouD.png)](https://imgtu.com/i/g8zouD)

**建议下载 [网易云极速版](https://www.lanzoux.com/iUw9Dheqpob)**

![04rmGR.png](https://s1.ax1x.com/2020/10/14/04rmGR.png)
此版本网易云功能简单稳定，与本软件兼容良好

<span style="color:orangered;font-weight:bold;">**方法二：**</span>请移步最下方观看有服务器自己搭建方案，然后手机上依次进入`设置`＞`WLAN `＞`修改网络`＞`高级选项`＞`代理    `，填写：ip地址+端口号/proxy.pac，例如：114.114.114.114:52000/proxy.pac

# <span style="color:orangered;font-weight:bold;">iOS端</span>

由于本人家境贫寒，买不起iPhone，无法截图说明，所以这里直接文字描述

请移步最下方观看有服务器自己搭建方案。

iOS端的使用也同样必须要连接WiFi，iOS 设备还需安装 CA 证书。首先点击**链接**：[https://raw.githubusercontent.com/nondanee/UnblockNeteaseMusic/master/ca.crt](https://raw.githubusercontent.com/nondanee/UnblockNeteaseMusic/master/ca.crt) 添加证书，随后在 `设置` > `通用` > `关于本机` > `证书信任设置` 下，手动开启证书，具体参考**Apple 官方说明**：[https://support.apple.com/zh-cn/HT204477](https://support.apple.com/zh-cn/HT204477) 。

安装后依次打开无线局域网＞HTTP代理＞配置代理，然后把代理选择为自动配置模式，同Android端一样，填写：ip地址+端口号/proxy.pac，例如：114.114.114.114:52000/proxy.pac，记得点击右上角的存储！！！

# <span style="color:orangered;font-weight:bold;">有服务器自己搭建</span>

<span style="color:orangered;font-weight:bold;">**Windows系统服务器：**</span>

**纯文字教程：**

其实非常简单，就跟Windows端方法一一样，只需要在服务器上安装node.js，然后点开运行网易☁🎵.bat这个文件就可以了，然后去防火墙开放端口52000，网易云音乐代理服务器填服务器ip或者绑定服务器的域名，端口填52000就可以了。你也可以使用用宝塔面板的pm2添加项目直接运行就行了。如果你知道我在说什么，那么下面的图文教学就不用看了。

<span style="color:orangered;font-weight:bold;">**图文教学：**</span>

<span style="color:orangered;font-weight:bold;">**方法一：**</span>

**1.在服务器上安装node.js**

官方网站：[http://nodejs.cn/download/](http://nodejs.cn/download/)

下载后双击软件安装包打开安装，一直点下一步直到完成即可

![04G9vd.png](https://s1.ax1x.com/2020/10/14/04G9vd.png)

**2.下载项目源码：**[https://github.com/meng-chuan/Unlock-netease-cloud-music/archive/refs/heads/master.zip](https://github.com/meng-chuan/Unlock-netease-cloud-music/archive/refs/heads/master.zip)

下载后解压到任意文件夹,双击点开Unlock-netease-cloud-music文件夹中名为：网易☁🎵.bat 的文件

![04GpgH.png](https://s1.ax1x.com/2020/10/14/04GpgH.png)

注：此窗口不可关闭，可以最小化

**3.打开自己电脑上的网易云音乐客户端，进入设置页面，设置自定义代理：**

- 自定义代理 ：填写服务器地址和端口号

- 代理服务器地址：填你自己的服务器ip或者绑定服务器的域名

- 代理服务器端口：52000

  ![04GPKA.png](https://z3.ax1x.com/2021/05/08/g85Jjx.png)

以后都不用再管了。

<span style="color:orangered;font-weight:bold;">**方法二：**</span>

**1.提前把项目源码下载到服务器上，然后解压**

项目源码下载地址：https://lesskiss.lanzoui.com/b00oj1s2f 密码:6666

**2.服务器上安装宝塔软件：**

前往宝塔官网安装宝塔软件：[https://www.bt.cn/download/windows.html](https://www.bt.cn/download/windows.html)

点击立即下载

[![g8ImRA.png](https://z3.ax1x.com/2021/05/08/g8ImRA.png)](https://imgtu.com/i/g8ImRA)

然后打开下载好的软件，一键安装

[![g8IBZT.png](https://z3.ax1x.com/2021/05/08/g8IBZT.png)](https://imgtu.com/i/g8IBZT)

安装好后直接点击打开面板

[![g8o678.png](https://z3.ax1x.com/2021/05/08/g8o678.png)](https://imgtu.com/i/g8o678)

然后输入你的账号和密码进行登录

[![g8oTBV.png](https://z3.ax1x.com/2021/05/08/g8oTBV.png)](https://imgtu.com/i/g8oTBV)

**3.宝塔面板上直接部署：**

登录进去以后直接点击软件管理，搜索pm2，直接安装

[![g8TE3d.png](https://z3.ax1x.com/2021/05/08/g8TE3d.png)](https://imgtu.com/i/g8TE3d)

安装好后打开设置，点击node版本，随便安装一个版本

[![g8TGgs.png](https://z3.ax1x.com/2021/05/08/g8TGgs.png)](https://imgtu.com/i/g8TGgs)

然后点击项目列表，点击添加项目，添加你下载好的文件夹就可以了，然后点确定

[![g8H2tO.png](https://z3.ax1x.com/2021/05/08/g8H2tO.png)](https://imgtu.com/i/g8H2tO)

**4.开放端口：**

前往安全，放行端口

[![g8qiqI.png](https://z3.ax1x.com/2021/05/08/g8qiqI.png)](https://imgtu.com/i/g8qiqI)

**5.打开自己电脑上的网易云音乐客户端，进入设置页面，设置自定义代理：**

- 自定义代理 ：填写服务器地址和端口号

- 代理服务器地址：填你自己的服务器ip或者绑定服务器的域名

- 代理服务器端口：52000

  ![04GPKA.png](https://z3.ax1x.com/2021/05/08/g85Jjx.png)

以后都不用再管了。

<span style="color:orangered;font-weight:bold;">**Linux系统服务器：**</span>

**纯文字教程：**

直接用宝塔面板的pm2运行吧，简单粗暴。如果你不知道我在说什么，请看下面的图文教程

**图文教程：**

用Linux服务器的应该都有些基础，我这里就简单过一下吧。首先你要SSH远程到服务器，然后执行安装命令，去宝塔官网找对应的安装命令复制吧：[https://www.bt.cn/bbs/thread-19376-1-1.html](https://www.bt.cn/bbs/thread-19376-1-1.html)：

[![g8L3Xd.png](https://z3.ax1x.com/2021/05/08/g8L3Xd.png)](https://imgtu.com/i/g8L3Xd)

安装完成后会给你一个面板地址，账号和密码，直接在浏览器上远程登录即可

![g8oTBV.png](https://z3.ax1x.com/2021/05/08/g8oTBV.png)

登录进去以后点击文件，上传，选择提前下载并解压好的项目文件夹直接上传

[![gGVTAK.png](https://z3.ax1x.com/2021/05/08/gGVTAK.png)](https://imgtu.com/i/gGVTAK)

然后去软件商店搜索安装pm2，然后设置

![g8TE3d.png](https://z3.ax1x.com/2021/05/08/g8TE3d.png)

点击Node版本，随便安装一个版本

[![g8LyBn.png](https://z3.ax1x.com/2021/05/08/g8LyBn.png)](https://imgtu.com/i/g8LyBn)

然后去项目列表添加项目

[![g8Omuj.png](https://z3.ax1x.com/2021/05/08/g8Omuj.png)](https://imgtu.com/i/g8Omuj)

前往安全，放行端口

[![g8qiqI.png](https://z3.ax1x.com/2021/05/08/g8qiqI.png)](https://imgtu.com/i/g8qiqI)

打开自己电脑上的网易云音乐客户端，进入设置页面，设置自定义代理

- 自定义代理 ：填写服务器地址和端口号

- 代理服务器地址：填你自己的服务器ip或者绑定服务器的域名

- 代理服务器端口：52000

  ![04GPKA.png](https://z3.ax1x.com/2021/05/08/g85Jjx.png)

以后都不用再管了。

教程到此结束，喜欢我的作品请帮忙点个⭐，谢谢！！！



# 总结

如果有服务器，强烈建议自己搭建，安全稳定高效。

教程到此结束，喜欢我的作品请帮忙点个⭐，谢谢！！！

# 常见问题：

1.有没有搭建好的免费代理服务器可以使用？

答：唉！穷！我已经没有钱给你们搭建服务器了，目前自用的服务器是前段时间活动216元3年的腾讯云，本身服务器水管就小，目前就和身边的朋友一起用，用的人多了服务器根本跑不动。

2.就想白嫖搭建好的免费代理服务器怎么办？

答：你可以网上找找，有别人搭建好的，但是我这边不能保证安全性。

3.图文教程也看不懂，但是又想用怎么办？

答：看见下面的二维码了吗，打钱(疯狂暗示)，备注联系方式。

文末再向为本项目提供技术支持的开源项目致敬

[trazyn/ieaseMusic](https://github.com/trazyn/ieaseMusic)

[listen1/listen1_chrome_extension](https://github.com/listen1/listen1_chrome_extension)

[EraserKing/CloudMusicGear](https://github.com/EraserKing/CloudMusicGear)

[EraserKing/Unblock163MusicClient](https://github.com/EraserKing/Unblock163MusicClient)

[ITJesse/UnblockNeteaseMusic](https://github.com/ITJesse/UnblockNeteaseMusic/)

[bin456789/Unblock163MusicClient-Xposed](https://github.com/bin456789/Unblock163MusicClient-Xposed)

[YiuChoi/Unlock163Music](https://github.com/YiuChoi/Unlock163Music)

[yi-ji/NeteaseMusicAbroad](https://github.com/yi-ji/NeteaseMusicAbroad)

[stomakun/NeteaseReverseLadder](https://github.com/stomakun/NeteaseReverseLadder/)

[fengjueming/unblock-NetEaseMusic](https://github.com/fengjueming/unblock-NetEaseMusic)

[acgotaku/NetEaseMusicWorld](https://github.com/acgotaku/NetEaseMusicWorld)

[mengskysama/163-Cloud-Music-Unlock](https://github.com/mengskysama/163-Cloud-Music-Unlock)

[azureplus/163-music-unlock](https://github.com/azureplus/163-music-unlock)

[typcn/163music-mac-client-unlock](https://github.com/typcn/163music-mac-client-unlock)

https://github.com/nondanee/UnblockNeteaseMusic

https://github.com/ndroi/easy163

感谢大佬们默默无闻的付出，在下只是大自然的搬运工

# 本教程仅用于学习交流，如有侵权请联系本人删除，禁止他人用于非法用途，转载请注明出处，谢谢！！！

**注：如加载缓慢可前往本人码云项目查看**[https://gitee.com/meng-chuan/Unlock-netease-cloud-music](https://gitee.com/meng-chuan/Unlock-netease-cloud-music)

**码字不易，欢迎各位金主大大打赏**

![0gr7L9.png](https://s1.ax1x.com/2020/10/11/0gr7L9.png)