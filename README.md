# QQRedPackHelper

[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](LICENSE)
[![README](https://img.shields.io/badge/README-中文-blue.svg)](README-Chinese.md)

Mac系统下的QQ抢红包神器，支持群和个人红包，包括文字口令红包。

## V2.3

修复bug:
> 1. 抢到红包消息通知多次弹出问题。

功能：
> 1. 新增助手配置界面。
> 2. 新增抢红包群过滤。
> 3. 新增红包关键字过滤。
> 4. 新增抢红包随机范围内时间延迟。
> 5. 新增一种注入的脚本（为了解决签名版QQ和未签名版消息历史记录不一致和本地表情加载失败问题）。
> 6. 新增是否抢个人红包开关，默认为打开状态。

## V2.21
> 参考Mac微信助手的安装脚本，更改安装方式，新增插件卸载脚本，已支持APP Store应用商店下载版本注入。

## V2.2
修复bug：
> 1. 最近一条消息不能显示的问题。
> 2. 然后优化了助手设置界面，改为菜单栏方式设置。
> 3. 新增消息防撤回功能，可以在菜单栏进行设置。

## 安装

### 方式1
打开控制台窗口，执行Other目录中的`Install.sh`文件，如：`sh Install.sh`

### 方式2

打开控制台窗口，执行Other目录中的`SignatureInstall.sh`文件，如：`sh SignatureInstall.sh`，然后关闭控制台，再新打开一个控制台，
输入QQ或是qq都可以启动注入后的应用程序。
注意：这种方式注入启动，不会破坏QQ自身的签名，这是为了消息历史记录不一致和本地表情加载失败问题。

## 卸载
> 1. 打开控制台窗口，执行Other目录中的`Uninstall.sh`文件，如：`sh Uninstall.sh`，只针对采用方式1安装卸载！
> 2. 采用方式二安装，需要手动去 `/etc/profile`目录删除下面两行代码： 
```
alias qq='sh /Applications/QQ.app/Contents/MacOS/injectionQQ.sh'
alias QQ='sh /Applications/QQ.app/Contents/MacOS/injectionQQ.sh'
```

## 效果图

图 1-1

![](https://ws3.sinaimg.cn/large/006tKfTcgy1fpem7ygxofj30hd0nin0d.jpg)

图 1-2

![](https://ws1.sinaimg.cn/large/006tKfTcgy1fpem9bv7kzj30ie0olgop.jpg)
 
## 功能:
> 红包自动抢？ 支持群和个人红包，包括口令-文字红包，自动执行抢操作。
> 有朋友撤回消息，你想看吗？新增消息防撤回功能。
> 每次都要去点击左上角的关闭按钮，是不是很烦？现在新增红包弹框自动关闭功能。

## 注意：
1. 助手设置选项现在直接放在顶部的菜单栏中啦，设置更加方便  
2. 想要自己编译项目，需要安装 [MonkeyDev](https://github.com/AloneMonkey/MonkeyDev)
3. 测试QQ版本截图：

![](https://ws1.sinaimg.cn/large/006tNc79gy1fozoyuhihej30dw09bgly.jpg)  