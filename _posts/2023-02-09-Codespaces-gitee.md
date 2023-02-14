---
title: Codespances使用git提交到gitee
img_path: /assets/img/posts/20230209/
categories: [奇技淫巧]
tags: [Codespances, git, gitee]
---

本文讲解在 Codespances(<https://github.com/codespaces>) 工具中如何提交代码到 gitee 仓库

_使用 github 库创建 Codespances 空间(不需要任何配置直接就能提交到 github)_

### 向 gitee 添加 ssh 密钥

1. 创建 ssh 密钥方式 gitee 进行验证 (https 方式未尝试成功)
    ```shell
    cd ~/.ssh/ #转到.ssh目录
    ssh-keygen -t ed25519 -C "xxxxx@xxxxx.com" #创建ssh密钥
    # *敲三次回车(默认参数都为空),之前我输入一些参数后创建的密钥验证不过
    cat ~/.ssh/id_ed25519.pub #查看公钥
    ```
2. 向 gitee 添加 ssh 公钥,点这个连接去配置 <https://gitee.com/profile/sshkeys>
    ```shell
    ssh -T git@gitee.com #测试配置是否成功
    #成功显示 Hi XXX! You've successfully authenticated, but Gitee.com does not provide shell access.
    ```
3. 如果出现错误 :
    > git@gitee.com: Permission denied (publickey)
    {: .prompt-danger }

    请检查上述注意事项:创建密钥时参数都为空、添加 gitee 公钥不要在仓库添加 

### Codespances 中 git 操作
1.  git add.

![gitadd](gitadd.png)

2. git commit

![gitcommit](gitcommit.png)

3. git push

![gitpush](gitpush.png)

4. 首次需要添加 gitee 地址 注意使用 ssh 连接
    - 输入 gitee 仓库的 ssh 连接=>回车
    - 输入远程仓库名称(随意)=>回车
    - 完成推送

![addremote](addremote.png)
