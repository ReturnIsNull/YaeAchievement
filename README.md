﻿<div align="center">

# YaeAchievement

![GitHub](https://img.shields.io/badge/License-GPL--3.0-brightgreen?style=flat-square) ![GitHub release (latest by date)](https://img.shields.io/github/v/release/HolographicHat/genshin-achievement-export?color=brightgreen&label=Release&style=flat-square) ![GitHub issues](https://img.shields.io/github/issues/HolographicHat/genshin-achievement-export?label=Issues&style=flat-square) ![Downloads](https://img.shields.io/github/downloads/HolographicHat/genshin-achievement-export/total?color=brightgreen&label=Downloads&style=flat-square) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)

</div>

- 支持导出所有类别的成就
- 支持官服，渠道服与国际服
- 支持导出至[椰羊](https://cocogoat.work/achievement)、[SnapGenshin](https://github.com/DGP-Studio/Snap.Genshin)、[Paimon.moe](https://paimon.moe/achievement/)、[Seelie.me](https://seelie.me/achievements)和表格文件(csv)
- 没有窗口大小、游戏语言等要求

## 使用说明
**打开程序前需要关闭正在运行的原神主程序**  
第一次打开需要先设置原神主程序(YuanShen.exe/GenshinImpact.exe)所在路径
![alt](https://upload-bbs.mihoyo.com/upload/2022/04/06/165631158/e540a5a6d50cd5fdee19665435548e00_514247033566841954.jpg)
### Windows7
系统变量添加名为```NODE_SKIP_PLATFORM_CHECK```的变量并将值设为```1```   
[[?]如何添加环境变量](https://www.bing.com/search?q=windows+7+环境变量)

## 下载地址
[releases/latest](https://github.com/HolographicHat/genshin-achievement-export/releases/latest)

## 问题反馈
[issues](https://github.com/HolographicHat/genshin-achievement-export/issues)或[QQ群: 913777414](https://qm.qq.com/cgi-bin/qm/qr?k=9UGz-chQVTjZa4b82RA_A41vIcBVNpms&jump_from=webapi)

## 常见问题
0. Q: 程序异常退出或被强行终止后，程序报错：网络错误(22-1) 或 原神启动时报错: 无法连接网络(4201)   
   A: 用文本编辑器打开```C:\Windows\System32\drivers\etc\hosts```，删除```127.0.0.1 dispatch**global.yuanshen.com```后保存，重启原神

1. Q: 原神启动时报错: 数据异常(31-4302)   
   A: 不要把软件和原神主程序放一起

2. Q: 为什么需要管理员权限  
   A: 临时修改Hosts和启动原神

3. Q: 报毒?   
   A: 执行命令或修改hosts引发，相关代码可在./utils.js,./appcenter.js下找到

4. Q: 原神进门后没有自动退出，程序输出停留在“加载完成”   
   A: 关闭代理后重试

5. Q: 网络错误，请检查网络后重试 (21-x)   
   A: 如果你是校园网用户，使用流量上网并重试；如果你是海外用户，打开config.json，将oversea_api的值设置为true并重试   
