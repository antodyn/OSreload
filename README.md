
# 系统重装保姆级教程V2.2


#### 文/张谨一


![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200401133744.jpg)


> **本教程PDF版下载地址：[www.lanzous.com/b034r918d](https://www.lanzous.com/b034r918d)**
> **密码:2vv2**
>
> 写给还不会装机的人： 对于没有接触过系统重装的人来说，装系统是一个很高端很难的事情。事实上，装机真的简单到不得了，我们只是把前人的劳动成果照搬而已，**所有装机用到的东西，都不是我们自己创作的，我们只是学会如何用而已**。
> 
> 因为硬盘分区表格式的不同，以及其他各种原因，**如果不去设置，Win7只能重装Win7，Win10只能重装Win10**。鉴于这是一篇傻瓜式教程，怎么修改BIOS以及硬盘分区表格式等等这次暂时不教，先学会重装。**如果你真的很需要，百度有全面的教程，照做一般没啥问题**。
> 
> 如果你只是想重装系统，请继续往下翻，如果你想win7换win10，或者电脑出了问题以下方法不适用，请往下翻参照：**【教程五】Win10万能恢复**
>

## 目录索引
[TOC]

------

## 【教程一】Windows系统重装


### 前言
#### 一般来说，有3种装机方式
1. 使用PE盘安装，用制作工具将U盘里装入一个PE系统（精简版Windows），然后重启电脑进入U盘，用PE系统里自带的工具，来完成重装。

   * 相比起其他方式，PE U盘装机的好处是可以随时随地给任何电脑装机，可以通过PE系统里的工具进行分区、引导修复、密码清除等等，同时因为可以访问硬盘，在你系统崩溃的时候，抢救出原系统里的文件。

   * 常用的PE制作工具有：
     * 无广告无捆绑的：微PE，优启通；
     * 有广告有捆绑但可以关闭的：电脑店；
     * 有广告有捆绑的：大白菜老毛桃等等
     
   * PE盘的制作过程中会格式化U盘，所以建议选一个空白U盘，或者先将U盘文件拷出，制作完成之后再拷入。**制作完成的PE盘完全可以当普通U盘来使用。**

   * **推荐直接使用微PE，公认的最好用的PE系统**

      

2. 用UltraISO等工具，将Windows镜像文件(ISO格式)刻录到U盘；或者使用微软官网提供的工具刻录U盘。之后依然是重启电脑进入U盘，这种方法原汁原味，安装过程和买到的正版Windows光盘的安装方法完全一样，缺点是没有各种PE工具，也**不能拯救电脑里的文件**。

   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331170928.png)

   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331170934.png)



3. 通过硬盘安装，即通过“小白一键重装系统”等类似工具，只需要电脑能开机就可以安装系统。最不推荐的方式，因为**一旦出现问题，电脑开不了机，你就只能去网吧或者找别的电脑，制作U盘来拯救。**

   

#### 重装完的系统还是正版吗？/我安装的系统是正版吗？

1. 首先要明确什么是正版：让开发者获得他认同的、合法的收益，你获得的软件服务才是正版。

2. 明确了什么是正版，那就清楚了：除了自己和公司购买的系统，或者买回的电脑自带的系统是正版，其他的都是盗版系统，包括某宝某多多买的，也是盗版系统。

3. 常见的激活方法
   * 如果你的电脑自带**家庭版**Win10，那么你重装了**家庭版**之后只要联网，就可以自动激活，**专业版和其他版本同理，只要安装同一版本就能自动激活**；
   * 通过**Win10数字权利激活工具**激活的系统，可以获得和正版一模一样的服务，比如重装之后联网自动激活、更新系统等等，不适用于Win7；
   * 通过**KMS激活工具**激活的系统，不可以重装激活，且激活时间一般为180天，大部分工具会在180后续激活，如果你的电脑在180天以内没有联网，KMS无法续激活成功，那么你的系统就崩了。Win7只能用KMS激活；
   * 通过某宝/某多多购买的密钥激活的系统，便宜的不可以重装，贵一些的可以重装，一定要问清楚卖家。（友情提示：翻看宝贝的评论区，查看评论区的图片，大概率可以白嫖到激活密钥）

   **谨一推荐的即为数字权利激活方式，虽然是盗版，但是和正版完全一样，大家可以放心使用。**

------



### 一、下载装机所需文件
#### 1. Windows系统：[msdn.itellyou.cn](https://msdn.itellyou.cn/)
进去之后从左边的列表里选择**"操作系统"**，然后找到最新版下载即可
比如我现在Win10的选择：

![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331170940.jpg)


  * consumer editions为消费者版镜像，包含家庭版和专业版等多个版本；business editions为商业版镜像，不包含家庭版，包含企业版和专业版等多个版本；这两个版本其实都可以，一般大家会下载消费者版。

  * 镜像文件名里的（x64）表示适用于64位电脑，建议4G内存以上，配置较好的电脑使用，（x84）适用于32位电脑，4G内存以下，配置较差、老电脑。

  * ed2k://开头的即为电驴下载链接，可以使用迅雷下载，也可以使用百度网盘离线下载功能离线到网盘里，再用网盘下载

    

  Win7的选择：一般大家使用的Win7都是带SP1补丁的旗舰版，如图中所示：
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331170946.jpg)



   Xp的选择：因为原版Xp装机过于繁琐，一般都使用Ghost系统，驱动和激活都能很好的解决。使用深度技术、番茄花园、雨林木风等等的**纯净版**Ghost Xp均可。



> 注意：
> MSDN2020年可能会启用新站**[next.itellyou.cn](https://next.itellyou.cn/)**，新站的界面更好看，但使用方法应该是类似的，大家灵活运用即可
>
> **非常不推荐大家使用Ghost系统**，即网上随处可见的纯净版、装机版、快速安装版等等，至于为什么大家可以自行百度“Ghost系统的坏处”，**记住一点：用原版系统就是最安全的，最好用的！**



#### 2. 下载微PE刻录工具：[www.wepe.com.cn](http://www.wepe.com.cn/download.html)
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331170952.jpg)



#### 3. 下载显卡驱动

**非常不推荐高性能独显使用Win10自动安装的驱动，版本低，还会有各种奇怪的问题，除显卡外其他驱动可以不用在意**

**Nvdia英伟达显卡**：[www.nvidia.cn/Download/Find.aspx?lang=cn](https://www.nvidia.cn/Download/Find.aspx?lang=cn)

   * **目前Nvdia官网和Win10提供的驱动都是DCH驱动**，即不带Nvdia控制面板，需要自行到Win10应用商店下载，**不去下载安装就会一直弹窗**，同时也意味着Win7不能安装该驱动。目测这么干是为了劝退Win7用户，增加Win10应用商店活跃度。
     ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171302.png)

   * 标准版驱动（带Nvdia控制面板）的下载入口目前只有这个，请大家收藏上面的网址：
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331170957.jpg)



 **AMD显卡**：[www.amd.com/zh-hans/support](https://www.amd.com/zh-hans/support)



#### 4. 下载驱动工具
360驱动大师：[weishi.360.cn/qudongdashi](http://weishi.360.cn/qudongdashi/)
比起驱动精灵驱动人生等等，这个至少没广告和捆绑软件，算是可以用一用，**但在用之前请你看完**：
   * 如果你是品牌笔记本，一般都有对应的驱动工具或者驱动下载地址，比如联想电脑都可以用联想驱动管理软件，戴尔电脑可以去戴尔官网按机型查询驱动。**我们推荐你使用品牌方提供的驱动，因为这和你的电脑最为契合**
   * 如果是重装Win10，Win10会自动在联网时自动帮你补齐驱动，只要等待一会就可以。
   * 如果是重装Win7，Win7是无法自动补齐驱动的，所以一定要**提前下载网卡版驱动大师**。
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171002.png)

------



### 二、制作PE盘
1. 到[微PE官网](http://www.wepe.com.cn/download.html)下载好微PE之后插入U盘，运行微PE，点击右下角的安装到U盘
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171102.png)

2. 之后的设置直接默认即可，全能三分区方式基本可以支持所有的电脑，**制作过程中会格式化U盘**，所以建议选一个空白U盘，或者先将U盘文件拷出，制作完成之后再拷入。
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171106.png)

3. 如果你只是为一台电脑重装系统，系统镜像文件不用放入U盘，放到非C盘即可，如果你想为其他电脑重装，在制作完成后把镜像文件放入U盘，就可以很方便的为他人重装系统，**前提是U盘空间够大**。

4. 如果你不需要微PE U盘了，因为有三个分区，直接格式化可能会有问题，一个比较好的方法是**先用微PE里的单分区方式再制作一次，然后再格式化**，就可以完美还原。

------



### 三、进入U盘 PE系统
开机之后，在看到电脑品牌LOGO是立即连续不断的敲击F12，进入F12 快速选择界面（各型号电脑进入方式不同，请自行百度**“电脑型号/主板型号+设置U盘第一启动）**，选择自己的U盘，一般有**“USB”字样或者是U盘品牌**：

比如我这里选的是我的金士顿Kingston U盘：
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171111.jpg)

------



### 四、开始重装系统
1. 在PE系统里点击**“CGI备份还原”**，然后在第二项里选择自己要装系统的盘，请根据大小来判断哪个是你的C盘，不要根据盘符来判断：

![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171118.jpg)

2. 在CGI备份还原的第三项里选择自己下载的系统镜像文件，然后会弹出系统版本选择界面，Home即为家庭版，一般选择Pro专业版，大家按需选择：

![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171122.jpg)

3. 然后就可以点击执行，在进度条结束之后，拔掉U盘，重启电脑，就可以进入新系统，重装完成。
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171126.jpg)

4. 如果你调整或删除了系统盘的隐藏分区，比如很多人为了干净，会选择删除所有分区，或者使用了新的没有安装过系统的硬盘，可能会遇到重启之后无法进去系统的情况，请往下翻参照：**【教程四】无法引导系统解决办法**

5. Xp系统因为推荐使用纯净版Ghost系统，在安装系统时请选择**“Ghost备份还原”**，其余操作与上面的步骤是类似的。

------



### 五、系统激活
1. 开头的前言里我们讲明白了正版盗版的问题，和各种激活方式的不同，**没仔细看的同学请到前言里仔细看。如果你是自带的Win10家庭版且重装的也是家庭版，联网等一会就可以自动激活。**

2. Win10数字权利激活工具和KMS工具（支持Win7）我已经上传到了网盘里，大家自己下载使用即可。**但是在使用前请先看【教程二】第一步“暂时关闭Defender”，否则你的工具会在解压后消失不见，只留下一个空文件夹**

   度盘：
   链接: [pan.baidu.com/s/1QmPmeEJeyW--bvGJngA3pQ](https://pan.baidu.com/s/1QmPmeEJeyW--bvGJngA3pQ)  
   密码: f898

   蓝奏云：
   链接: [www.lanzous.com/b034r543c](https://www.lanzous.com/b034r543c)
   密码: 6o1w

3. Win10激活的时候，有时候工具会提示“**Windows处于通知模式**”，具体原因谨一也没细研究过，不过百度可以找到解决办法，嫌麻烦的同学可以到某宝/某多多直接购买激活密钥，多看评论区的图片还有机会白嫖。

4. 检验激活状态
此方法适用于Win10和Win7
   * 按下Win键+R，打开运行（打开运行的方法很多随便你用哪个）
     
     ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331180206.png)
   
   * 输入引号里的代码，注意vbs和-之间有一个空格：**“slmgr.vbs -xpr”**
   
   * Win10使用了数字权利工具、使用了购买的密钥、Win7使用了购买的密钥，会提示**“计算机已永久激活“**
     ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331180213.png)
   
   * Win10或Win7使用了KMS激活工具，会提示“批量激活将于XXX过期”，不过会有自动续激活，也就是只要一直联网就可以一直激活状态。**在用第三方工具关闭启动项的时候注意不要关闭和KMS有关的计划任务。**

------



### 六、驱动安装

#### 1. Win10
   * 进入系统之后一般只安装显卡驱动就好了，其他驱动可以等联网状态自己安装，也可以用品牌方的工具安装，不建议使用第三方工具安装。
   
   * **N卡用户请看**：如果因为网速过快，Win10已经安装完了独显DCH驱动，这时候你每次开机都会在右下角弹窗“**NVDIA Control Panel is not found**”
     
     ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171302.png)
     
      **解决办法有三：**
     
     * 打开Win10应用商店，登陆微软账户，搜索“**NVDIA Control Panel**”安装即可解决。
     * 先断开网络，在控制面板-卸载程序 或者 设置-应用 里，选中NVDIA相关的软件全部卸载。重启之后安装**第三步第3条**里下载的标准版显卡驱动，就解决了，之后可以联网。
     * 在系统装完，**开始配置系统还未进入桌面时**，拔出网线不要连Wi-Fi，Win10就不会装驱动，装完标准版驱动再联网安装其他驱动。

#### 2. Win7
Win7不会自动安装驱动，但也意味着不会自动安装网卡驱动，就是不能上网，所以一定要提前将**第三步第3条**里下载的显卡驱动和万能网卡版驱动大师放到U盘里。



## 【教程二】系统初步优化
**很多人喜欢Ghost系统的原因之一是Ghost系统做了所谓的优化，但事实上并不一定，Ghost作者并不知道你的具体配置，他甚至无法知道你用的是N卡还是A卡，又何来优化一说。**

系统优化这件事其实核心就一个：符合自己的需求，因此下面的教程基本都是必做项，不完整但是挺有用。**如果你是大佬，请直接忽略本教程二，如果你对电脑不熟悉，可以跟着做一做。**



### 一、暂时关闭Defender
Windows Defender是Win10自带的杀毒软件，**比起各种免费的杀毒软件，在保护电脑安全上它靠谱的多**，毕竟是微软自家的系统，自家的杀毒软件。这一点大家可以自行百度。我们关闭DF的原因很简单：**它会删除我们的系统激活工具，软件破解工具等等**，对于一个天朝人来说它并不是那么的友好。

   * 如果你不需要用到各种破解软件，完全可以再激活系统后重新打开它，不需要再安装其他免费的杀毒软件。Defender完全够用！如果不够用说明你看片太多了，节制一点。
   * 如果你接受不了误删你的文件，或者经常接触危险文件。可以关闭之后使用火绒、小红伞Avira、Avast、卡巴斯基免费版等等。
   * **对病毒最好的防范不是安装好的杀毒软件，而是不下载危险文件。**

#### 关闭方法：
1. 打开设置-更新和安全-Windows安全中心-病毒和威胁防护

   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171134.png)

2. 点击病毒和威胁防护设置下方的“管理设置”

   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171139.png)

3. 将所有的开关都关闭，Defender就不会再误删你的文件。

   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171143.png)



### 二、找出桌面图标
这简直是最简单的一步，但却是很多人都困扰的一步，因为重装完成之后自己的桌面上就一个回收站？？？

1. 右击桌面-个性化

2. 选择主题-桌面图标设置：
   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171147.png)


3. 勾选你需要的图标，应用之后桌面上就会出现了
   
   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171152.png)



### 三、释放电脑性能
请务必在跑分之后删除鲁大师之类的软件，你花了钱买回来的电脑不是要节能模式省电的，**而是要在不损伤硬件的前提下享受它的性能的**。

如果你实在想用鲁大师检测运行游戏时电脑的状态，温度帧数等等，GamePP（游戏加加）是个好选择



#### 1. CPU内存超频（笔记本电脑请忽略）

这一部分我不会详细教，因为每个主板的设置方法都不一样，大家自己搜索“品牌+CPU超频设置”、“品牌+内存超频设置”慢慢学习。

这里我只提供一下思路：
   * 先查一下你的CPU型号大家都能超频到多少稳定，适当降0.1-0.2，比如大家都能超到4.9Ghz稳定，那你超到4.8、4.7就没啥问题。
   * 现在的CPU超频大多数是只改倍频，外频默认100Mhz不动，比如倍频48就是CPU4.8Ghz。
   * 大部分内存都可以升一个档次或两个档次，体质好的可以升三个档次，比如现在DDR4的内存频率一般都是2133、2400、2666、3000、3200等等，颗粒越好能超的越多。
   * 如果你买的内存频率是高于2666的，插到电脑上也只是默认2666，需要你选择X.M.P配置文件或者自己超到高频率，否则只会以2666频率运行。

**非常不建议笔记本进行超频，即便你的CPU可以超。因为笔记本性能的瓶颈是散热问题，超频可能会导致温度压不住，造成不可挽回的损失。**



#### 2. 关闭主板节能模式
笔记本电脑一般没有这个选项。

各个主板的设置方法不一样，AMD平台一般都有，Intel平台较少，大家自己查找即可。

如果你进行了超频，记得进行“**防掉压设置**”。



#### 3. 打开系统高性能模式
   * 打开控制面板，在右上角将查看方式改为小图标

     ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171155.png)

   * 找到电源选项

     ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171159.png)

   * 点击右边的下拉箭头打开隐藏附加计划，选择“高性能“，**如果这里没有高性能选项也可以到左边”创建电源计划“自己创建一个**

     ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171205.png)


   * 如果你是N卡：右击桌面-NVDIA控制面板-将“**设置PhysX配置**”选择为你的独立显卡，然后右下角点击应用；**如果你是N卡笔记本，还需要在“管理3D设置”里将首选图形处理器选为“高性能NVDIA处理器”**，然后右下角点击应用。

     


### 四、关闭启动项
**你可以先安装你要用的软件，安装差不多了再来关闭启动项。**

关闭你不需要的启动项不仅可以防止一开机就弹出一大堆应用，还能加速开机时间，减少电脑开机时候的卡顿情况。

打开控制面板，到“启动”这一页里就可以关闭你不需要的启动项，你也可以用第三方软件来管理启动项：
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171209.png)



### 五、关闭弹窗

目前针对弹窗没有什么特别好的完全清理方法，只能做到拦截。
   * 如果是在屏幕正中出现的广告弹窗，一般弹窗里会有设置按钮或者三道杠按钮，点开里面会有“不再弹出”“永久关闭”等选项。

   * 如果是在右下角出现的广告弹窗，一般会有“不再提示”可以勾选，勾选后关闭就不会再弹出。

   * 爱奇艺优酷等等的广告，在软件设置里可以关闭弹窗。

   * 火绒等安全软件会有弹窗拦截小工具，用起来效果还算不错。



## 【教程三】系统备份与还原

**每一次重装都很麻烦，要设置很多东西，最好的方法就是在重装完毕，优化完毕之后，直接进行一次备份，如果以后有什么问题，直接还原就可以了。**

### 一、备份
我们这里不使用Windows自带的备份还原，因为有更加方便快捷省事的方式

1. 下载软件Dism++：[www.chuyu.me/zh-Hans/index.html](https://www.chuyu.me/zh-Hans/index.html)

2. 解压运行，64位系统运行“Dism++x64”，32位系统运行“Dism++x86”

3. 打开软件后选择工具箱-系统备份

   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171214.png)

4. 点击“浏览”，选择生成的备份文件的存放路径（确保这个路径的空间要比你现在C盘的已使用空间要大），然后在文件名一栏里给备份文件起一个名字，建议以时间为命名方式

   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331173803.png)

5. 点击保存、确定之后就会开始备份，可以看到进度条。备份速度是先慢后快的，C盘越大越慢。

   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171218.png)

6. 备份完成会生成一个.wim格式的文件，你可以把此文件放到C盘以外的其他盘或者移动硬盘安全保存。

   

### 二、还原
上面生成的wim文件既可以给你的电脑还原，也可以给其他电脑（但是不建议，除非配置一样）
1. 插入微PE U盘，从U盘启动电脑。

2. 打开CGI备份还原，选择你的系统盘，镜像文件选择你的wim格式的备份文件，整个步骤和重装系统是一样的，具体请查看【教程一】第四步。
   
   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171221.jpg)

3. 还原完成重启进入电脑，你会发现C盘被恢复到了备份时候的样子，文件布局、各种设置都一模一样。



## 【教程四】无法引导系统解决办法

如果调整或删除了系统盘的隐藏分区，比如很多人为了干净，会选择删除所有分区，或者使用了新的没有安装过系统的硬盘，可能会遇到重启之后无法进去系统的情况。

这时候有两个方法来解决：

### 一、自助建立ESP和MSR分区

1. 在PE盘里打开分区助手，找到系统盘对应的那块硬盘，先删除所有分区，会变为一块未分配的空间，然后再建立一个新分区，点左上角提交（**分区助手里必须提交才能生效**）

2. 点击分区助手上方的“快速分区”，根据自己的需要选择分区数量和各个区的大小，不想分区就在分区数目里选择“1”

3. **在“磁盘的类型”里选择“GPT”，勾选“创建ESP和MSR分区”，选择分区对齐到“4096扇区”**，然后开始执行分区，一般来说分区完成之后就可以正常安装系统，**如果还是不行，请尝试方法二**
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171225.jpg)



### 二、使用传统Windows安装方法自动建立
**如果你使用了【教程一】前言里系统重装方法二，请直接从第3步开始看**

1. 在PE盘里找到你的系统镜像文件，右击“加载ImDisk虚拟光驱”，加载设置直接默认就行，然后PE系统的此电脑里就会多出一个CD驱动器。
   
   ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171230.jpg)

2. 打开CD驱动器，运行“setup.exe”，就可以开始传统的Windows安装方式：
    ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171234.jpg)

3. 这一步点击下方的**“我没有产品密钥”**就可以跳过，我们可以在系统安装完成之后再用工具激活。
    ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171238.jpg)

4. 这一步请务必选择**“自定义：仅安装Windows”**，图片里的框请忽视：
    ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171242.jpg)

5. 这一步请先将所有的磁盘都删除，操作方法：挨个选中磁盘，点击“**删除**”，直到磁盘变成一块未分配的空间，然后点击“**新建**”，默认大小即可，系统会提示“**若确保Windos所有功能都正常，Windows可能要为系统文件创建额外的分区**”，即创建ESP和MSR分区，确定即可

    ![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171247.jpg)

6. 然后选择要安装系统的盘，就可以正常安装了，安装完成重启会进入新系统。

    


## 【教程五】Win10万能恢复
除去前面讲的正常装机外，还有一种装机方法，可以忽略硬盘格式，BIOS设置等等，简单快速的让电脑恢复到一个全新的Win10系统

代价：
   * 硬盘重置，所有文件丢失，硬盘分区合并。
   * 只能恢复为Win10系统，且为旧版Win10，需要后续自己更新。

**使用此方法不需要任何的设置，你只需要刻录好U盘，插上去就可以开始安装系统**，只要你的电脑硬件没问题，都可以装为Win10系统，非常适合电脑被自己搞坏，普通方法无法重装，还有Win7想换Win10的同学。

1. 下载所需文件
链接: [pan.baidu.com/s/16l-3G3V2SR1wQHAGhjwNNg](https://pan.baidu.com/s/16l-3G3V2SR1wQHAGhjwNNg)  
密码: pkcf

2. 解压下载好的UltraISO，运行“UltraISOPortable.exe”，点击“文件”-“打开”，打开下载好的恢复镜像：
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171251.png)

3. 插入U盘，点击“启动”-“写入硬盘映像”
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171254.png)

4. 选择好U盘，点击“写入”即可，如果软件卡住不动请耐心等一会：
![](https://raw.githubusercontent.com/ningcheers/PictureBed/master/PicGo/20200331171258.png)

5. 刻录完成之后，将U盘插入要恢复的电脑，进入U盘，进入方法请看【教程一】的第三步

6. 进入U盘后选择提示选择键盘布局，选微软拼音即可，然后依次点击**“疑难解答”-“从驱动器恢复”-“仅删除我的文件”-“恢复”**，就可以自动安装，安装完成自动进入新系统。







#### 文/张谨一
#### 欢迎转载，转载请注明作者及出处
#### 本教程PDF版下载地址：[www.lanzous.com/b034r918d](https://www.lanzous.com/b034r918d) 密码:2vv2
