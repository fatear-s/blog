---
title: githubblog
date: 2024-11-10 22:10:38
tags:
---

# github blog pages error&solve

## get github pages

url:https://pages.github.com/

## nodes.js、hexo、主题

https://gitcode.csdn.net/65aa2e27b8e5f01e1e44c4da.html?dp_token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpZCI6NDE3NDY2OSwiZXhwIjoxNzMxNzU5OTczLCJpYXQiOjE3MzExNTUxNzMsInVzZXJuYW1lIjoicXFfNDU5NDE4NjYifQ.r6fm4uOpnxdFaKUjo6FtxG7PEAbyWyxLKbWn3FZHoVM&spm=1001.2101.3001.6650.4&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7Ebaidujs_baidulandingword%7Eactivity-4-119089190-blog-142594777.235%5Ev43%5Epc_blog_bottom_relevance_base3&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7Ebaidujs_baidulandingword%7Eactivity-4-119089190-blog-142594777.235%5Ev43%5Epc_blog_bottom_relevance_base3&utm_relevant_index=9

## git 问题

### 添加SSH

```bash
ssh-keygen -t rsa -C "@qq.com"
# 将SSH key 添加到 ssh-agent
ssh-add id_rsa
#如果出现“Could not open a connection to your authentication agent.”的错误
eval "$(ssh-agent -s)"
ssh-add id_rsa
#验证key
ssh -T git@github.com 
```

将SSH key 添加到你的GitHub账户

![img](/images/githubblog1.png)

链接

https://blog.csdn.net/m0_69057918/article/details/132139286

### 更换分支

```bash
git pull --rebase origin main
```

链接

https://www.bilibili.com/opus/464126252045553313

### 提交代码

```bash
git init
git add .
git commit -m "blog"
git remote add origin git@.com
git push origin main/git push -u origin main
```

链接

https://zhuanlan.zhihu.com/p/675458343

