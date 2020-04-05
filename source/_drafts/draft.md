---
title: 彻底解决Mac下android调试模式adb经常断开的问题
categories:
  - 码农搬砖
tags:
  - android调试模式 adb经常断开 Mac系统
---
## 首先建议更新下adb版本及系统版本
adb --version  可以查看当前adb版本
homebrew升级可以参考
brew cask reinstall android-platform-tools

## 如果仍然有问题，可以尝试重置系统管理控制器 (SMC)--这个可以彻底解决adb连接自动断开
方法是关机后按住内建键盘左侧的 Shift-Control-Option，然后同时按下电源按钮。按住这些按键和电源按钮 10 秒钟；然后再开机。
详细可以参考官方文档
重置 SMC
https://support.apple.com/zh-cn/HT201295

## Mac下其他异常问题，可以参考
送修Mac前 万能的两个自救方法：重置 NVRAM（PRAM）与 重置 SMC
如何重置 NVRAM
https://support.apple.com/zh-cn/HT204063