<div id="top"></div>

<!-- PROJECT LOGO -->
<div align="center">

<img src="https://raw.githubusercontent.com/justminer/GoMinerTool/main/image/slogo.png#gh-light-mode-only" alt="Logo" width="200" height="200">

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
<!-- ![Github stars](https://img.shields.io/github/stars/justminer/GoMinerTool.svg) -->

# GoMinerTool
  <p align="center">
    <h2>抽水恒定千分之3，无递增，纯转发不抽水</h2>
    <h3>Web操作界面，简单易用，小白也可轻松上手，支持ETH/ETC/BTC/LTC/CFX/RVN/ERG/XMR等多个币种；欢迎实测对比</h3>
    <img src="./image/jt1.png" alt="Logo">
    <a href="https://kdocs.cn/l/slPG1q488Trc"></a>
    Telegram交流群：<a href="https://t.me/+Qam442PoHcs0YmIx">https://t.me/+Qam442PoHcs0YmIx</a>
  </p>
</div>



Linux一件安装脚本：

```
bash <(curl -s -L https://raw.githubusercontent.com/justminer/GoMinerTool/main/linux-install.sh)
```
完整复制命令运行；默认帐号admin，密码admin123；设置好以后切记更改[帐号密码]！



#### 常见的如奶牛、茉莉、亚米等机型, 需要用ETH端口, 芯动系列或其他的机型请选择ETH(GetWork)端口；如果设备无法正常接入，不同类型的端口可以交替着试一下。




# 软件预览

<p id="preview"></p>
<img src="./image/jt1.png" alt="Logo">

#### 请注意你们后台的版本号；警惕被服务商内部人员更换高抽水后台，认准cu-btc前缀；
#### 可与各类破解版对比，看看哪家实际开发费最低；

#### 部分windows服务器端口不受安全组控制，需要到“windows管理工具”-“高级安全Windows Defender”-入站规则新建端口规则才可以！

<img src="./image/tinified/jt3.png" alt="Logo">
<img src="./image/tinified/jt2.png" alt="Logo">
<!-- <img src="./image/tinified/t5.png" alt="Logo"> -->
<img src="./image/tinified/t6.png" alt="Logo">
<img src="./image/tinified/t7.png" alt="Logo">
<img src="./image/tinified/t8.png" alt="Logo">
<img src="./image/tinified/t9.png" alt="Logo">

# Windows服务器安装
下载完后直接启动即可，程序自带进程守护

<a href="https://github.com/justminer/GoMinerTool/tree/main/Windows-64">下载地址</a>

# Linux服务器安装
root用户直接执行以下命令, 根据提示选择对应功能即可。
```
bash <(curl -s -L https://raw.githubusercontent.com/justminer/GoMinerTool/main/linux-install.sh)
```justminer
### 安装完成之后, 请立即修改登录账号、密码以及启动端口，防止被爆破。
<img src="./image/t12.png" alt="Logo">


本地加密隧道请前往https://github.com/justminer/GoMinerTool/tree/main/KENC 自行下载


#### 算力跑不够的常见原因

如果测试下来24小时均值和设置的差距过大的话, 比如设置抽百分之1, 均值却少了很多, 有很多原因会导致这种情况发生，需要自己一步步排查。

⑴设备出现问题，例如中转里某些设备无效率很高，这种情况通常是卡出问题了, 这种情况通常比较容易排查，在后台中找到高无效的设备，点开后看下日志里是否有很多POW相关的关键字，如果有的话那么就说明这台设备的硬件出问题了，导致无效引发算力偏低。

⑵本地中招，这个非常容易遇到但是不好排查，可以在后台里建立一个纯转发的端口，用纯转发的端口测试设备24小时均值，如果纯转发的端口24小时跑不够，那么大概率是本地中招，本地重新安装干净的系统解决。

⑶检查挖矿软件配置及内核配置，是否设置超过多少分钟没有成功提交重启内核；

⑷查看你服务器的硬件配置及软件带宽，看你服务器的网络是否占用超过60%以上，配置过低可能导致转发性能不足，导致重发及超时；



<!-- GETTING STARTED -->
<p id="install"></p>



<p id="question"></p>
<p id="about"></p>

___


# 免责声明
<p id="flsm">
开发者仅在技术及爱好的驱使下维护此软件，本软件仅验证技术过程。

用前请遵循当地法律，不允许的区域内禁止使用。

使用此软件造成的法律问题, 一概与软件作者无关。
</p>


# 联系我们

电报: [https://t.me/+Qam442PoHcs0YmIx](https://t.me/+Qam442PoHcs0YmIx)


<span id="uplog"></span>
# 更新日志

```
2022.08.31
修复被扫描导致的软件重启；增加更多小币种，FLUX支持无损模式

2022.08.20
观察者地址可以关闭手续费了
增加显示敏感操作的日志，以便排查

2022.08.15
所有老版本请更新到此版本，并及时修改[帐号]和[密码]

2022.08.09
增加了dcrn、dcr抽水
优化ETC、ERG、kaspa、bch里一个可能发生错误的问题；

2022.08.05
ERG抽水更稳定

2022.08.01
修复隧道本地端断电掉配置的问题，增加调试端口proxy（部分有问题的机器可选择此端口）
全新界面，优化了页面细节及主题

2022.07.17
增加了KENC端口的自定义RSA密钥(此功能仅适用于自己制作客户端, 平时不要配置, 否则会导致kenc端口无法正常连接)

2022.07.01
提升程序稳定性

2022.07.01
修改了添加端口时的部分币种介绍
kenc的推送地址改为加密地址，加密地址只有最新版本的kenc客户端支持, 如需此功能，需重新下载kenc客户端及最新版GoMinerTool

2022.06.23
匹配更多小币种

2022.06.21
[重要更新] 
ETH完美版本
略微提升了ETH在某些池子的算力
降低了亚米设备在ETH端口的无效
增加了BEAM抽水
修复了ERG无效率偏高的问题
修复了RVN无效率偏高的问题

2022.06.18
增加了端口统计的矩形视图, 看总量统计更方便些了
修复了某些小币种的算力统计
增加了LTC的抽水
增加SERO币种抽水
实装了所有支持小币种抽水的算力统计

2022.06.14
修复了抽水钱包数量>1时, 算力分配不均衡的问题

2022.06.13
增加了观察者链接, 编辑端口-高级设置即可打开此功能
修复了茉莉等芯片机连接ETH端口无法登录的问题
适当提升了一点点内存占用, 用来降低可能发生无效的概率
支持多个指定钱包替换至目标钱包
修复了ETC芯片机 A11及一些小币种无损模式下可能无法正常工作的 bug
修复了2.4.X版本抽水过多的问题
增加了指定钱包地址替换功能
增加了设备名称正则表达式过滤设置
修复了某些情况下算力统计失效的情况
适当调低了三倍左右内存占用, 现在单台设备占用500kB内存 
增加了CFX抽水
增加了ERG抽水
增加了RVN抽水
修复了某个可能导致ETC芯片机和ETH芯片机造成无效的地方
增加了对nicehash的支持

2022.06.06
修复了ETC芯片机相关问题

2022.06.05
更换了LOGO
 修复了BTC抽水过少的问题
引入了ETC无损机制
支持了ETC芯片机
更新了BCH的逻辑
端口日志内增加了断开日志

2022.06.02
完美版A11
增加了兼容模式, 一些币种或机型在工作一段时间后出现大量无效导致无法继续工作时可以尝试使用此模式
对BTC进行了优化, 无法抽水的BTC机型和矿池, 可以使用兼容模式来进行工作
对A11进行了优化, 如果是A11的机器, 端口请选择ETH芯片级及无损模式
更新了KENC, 所有使用KENC客户端的用户请下载最新KENC
开放了BTC统一钱包

2022.05.28
设置里增加了KENC配置推送
修复了页面上一些显示的问题
BTC现在支持了所有矿池
BTC引入了无损机制
实装了BTC算力统计
BTC增加了动态难度抽水

2022.05.19
修复了特殊情况下无损逻辑暂时失效的BUG
适当缩小了数据尺寸, 降低了3/1的内存占用

2022.05.13
ETH增加了动态难度抽水机制, 跨池也能抽到比例算力了
略微提升了凤凰内核的算力
修复了部分内核不显示名字和算力的问题

2022.05.12
增加了本地算力修改的功能
极大稳定了算力补偿机制，给你稳稳的幸福

2022.05.10
支持了芯动矿机，创建端口时选择ETH芯片机即可
修复了算力补偿机器的名称问题，微量的提高了双方算力
修复了网页修改端口导致ip黑名单丢失的问题

2022.05.09
大大降低了ETH的损耗
增加了难度统计

2022.05.03
大大减小了特殊网络环境下的算力损耗
干掉了幽灵设备
修复了矿池内机器合并为defualt的问题
修复了TEAMRED内核的相关问题
增加了KENC隧道协议
增加了软防CC策略
增加了IP黑名单功能
TOKEN超时切换到登录页自动保留了账号密码
修复了自定义配置中文无法保存的问题
修复了端口证书相关的问题

2022.04.21
修复BTC抽水导致目标机器算力低下的问题

2022.04.20
实装了BTC和BCH的抽水
自定义配置现在可以导入导出和跨平台保留了

2022.04.12
修复了抽水导致的断连bug
实装掉线提醒
修改了一些可能导致延迟增加的地方
支持了网页修改web访问端口
新的安全逻辑, 避免被扫
支持了修改账号
修改了部分内核导致名字乱了的问题

2022.04.10
大幅提升程序稳定性 

2022.04.04
大幅提升程序稳定性
重新开放了小币种的转发

2022.03.30
修复了本地算力浮动的问题
更加稳定持久的连接
支持了不同钱包不同比例抽水
开放了备用池
增加了端口日志
更温柔的抽水
修复了币印新的TLS地址无法连接的问题
增加了设备连接时长
增加了钱包、机器名搜索
修改了一个容易导致内存泄漏的地方, 程序更加稳固
修复了某些小币种自定义配置不生效的问题
新的安装脚本, 更方便管理, 支持了开机启动修改端口等功能

2022.03.21
完全有效的抽水份额
新的抽水逻辑
实装btc（待测试）
端口内设备有时候算力为0, 不用担心，显示的问题，如果担心的话可以观察内核输出，仅仅是显示问题 稍后会优化掉
现在增加了万分之一的开发费用

2022.03.12
可配置多个钱包
修改了开启抽水导致的份额丢失问题
新的获取任务逻辑, 获取份额数量更快了一些
增加了常用自定义配置管理
可以单独导出某个端口的配置
优化页面细节
显示正常的区间内份额统计图表
机器增加了日志,点击机器查看详情可看到（持续更新）
增加了一键默认配置
修改了sn冲突导致的无法登录的问题

2022.02.28
修改了内存爆炸的问题
修改了抽水钱包算力过多的问题
端口关闭下可以开关SSL以及重新配置证书
取消自动更新功能
去掉了无效的设置

2022.02.27
修复了导致软件崩溃的几个关键问题
修复了粘包导致的份额丢失的问题
修复了首次启动看不到图表的问题
抽水算法改为随机算法，曲线更稳定
增加了端口配置TLS证书功能
增加矿池连接状态测试功能
增加抽水份额统计
增加原始钱包地址查看登录页右下键可以查看机器码

2022.02.23
修改了抽水统一钱包失效的问题
修改了抽水逻辑，现在频率更高，矿池曲线更稳定
增加列表分页及设置
修正了某些情况下含有数据统计的币种也会提示未知设备的问题

2022.02.18
默认端口号改为16777
更换进程守护方式
页面优化
数据列表默认排序
修正更换端口无法启动的问题
可以正常转发但是不支持数据统计的币种，列表内现在可以显示设备了
增加抽水设备名称的配置
增加了矿池模式统一名称的配置
增加语言包

2022.01.31
稳定性改进
增加了一些ETH预置矿池
修复了目标矿池为SSL连不上的问题
```



<p align="right">(<a href="#top">back to top</a>)</p>


[contributors-shield]: https://img.shields.io/github/contributors/justminer/GoMinerTool.svg?style=flat
[contributors-url]: https://github.com/justminer/GoMinerTool/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/justminer/GoMinerTool.svg?style=flat
[forks-url]: https://github.com/justminer/GoMinerTool/network/members
[stars-shield]: https://img.shields.io/github/stars/justminer/GoMinerTool.svg?style=flat
[stars-url]: https://github.com/justminer/GoMinerTool/stargazers
[issues-shield]: https://img.shields.io/github/issues/justminer/GoMinerTool.svg?style=flat
[issues-url]: https://github.com/justminer/GoMinerTool/issues
[license-shield]: https://img.shields.io/github/license/justminer/GoMinerTool.svg?style=flat
