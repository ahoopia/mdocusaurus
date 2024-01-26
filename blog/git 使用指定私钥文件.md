---
title: git 使用指定私钥文件
tags: [工具,Linux]
---

git 下使用指定私钥实现 ssh 免密推送拉取需要以下配置
```bash
Host github.com
    HostName github.com
    User git
    IdentityFile #私钥路径，windows注意\
    IdentitiesOnly yes
```