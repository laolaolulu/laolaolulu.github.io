---
title: 2023年各大厂WebIDE(CloudStudio、DevStudio、Codespaces)使用对比
img_path: /assets/img/posts/20230213/
categories: [短中取长]
tags: [WebIDE, CloudStudio, DevStudio, Codespaces]
---

本人抱着颗白嫖的心态撸了一遍各大厂的 WebIDE(CloudStudio、DevStudio、Codespaces) 工具,现分享下白嫖经验

### 腾讯 CloudStudio

_<https://cloudstudio.net/>_

- 最花里胡哨的工具,建库很多模板有不同的操作系统(Red Ubuntu),模板没尝试完...
- 该有的环境常用的工具都安装好了(最新长期稳定版)
- 每月能白嫖 1000 分钟(所有仓库空间共用),然后 1 毛钱一分钟;包月 300

![addremote](cloudstudio-index.png)

![addremote](cloudstudio-code.png)

![addremote](cloudstudio-cost.png)

### 阿里 DevStudio

_<https://ide.aliyun.com/>_

- 目前为止处于测试阶段可以完全白嫖但不知道正式版收费如何
- 有完善的 java 开发环境
- 环境配置不完善,node 默认还是 12(自带版本管理工具),很多开发环境需要自行安装
- 空间停止(会自动)后重新进入你的任何配置都还原了

![addremote](devstudio-index.png)

![addremote](devstudio-code.png)

### 华为 CloudIDE

免费开通,结果我点了提示余额不足;我这个白嫖党为了感受华为带来的神秘感特意充值 1 元,结果还是余额不足放弃体验......

### 微软 Codespaces

_<https://github.com/codespaces>_

- 只能使用 github 仓库初始化(进去用 git 想怎么提交都行)
- 每月免费 60 小时,超出后 0.18 美元一小时 (1.23 元)
- 开发环境全是最新
- 基本上不需要做任何配置就能进行开发

![addremote](codespaces-index.png)

![addremote](codespaces-code.png)

![addremote](codespaces-cost.png)

### 总结

只体验了一遍通用开发环境,用 vs code 的推荐上手;没有完全白嫖的,建议国内大厂出个开源免费使用模式:例如使用自家的 git 仓库,开源库可免费使用;或者放大免费使用时间平均每天免费 4 小时左右...
