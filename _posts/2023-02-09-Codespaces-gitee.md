---
title: Codespances使用git提交到gitee
---

本文讲解在 Codespances(https://github.com/codespaces)工具中如何提交代码到gitee仓库

1. 使用 github 库创建 Codespances 空间(不需要任何配置直接就能提交到 github)
2. 创建 ssh 密钥方式 gitee 进行验证 (https 方式未尝试成功)

```shell
cd ~/.ssh/ #转到.ssh目录
ssh-keygen -t ed25519 -C "xxxxx@xxxxx.com" #创建ssh密钥 *敲三次回车(默认参数都为空),之前我输入一些参数后创建的密钥验证不过
cat ~/.ssh/id_ed25519.pub #查看公钥
```

3. 向 gitee 添加 ssh 公钥,这个连接去配置(https://gitee.com/profile/sshkeys)

```shell
ssh -T git@gitee.com #测试配置是否成功
#成功显示 Hi XXX! You've successfully authenticated, but Gitee.com does not provide shell access.
```

### Codespances 中 git 操作

```shell
git add.
```

![image](/assets/img/posts/20230209/gitadd.png)
