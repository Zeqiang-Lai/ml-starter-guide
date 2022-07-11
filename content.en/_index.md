# 👷 维护人员首页

首先，欢迎你加入维护团队😆

接下来，我们一起跟随着这份文档学习如何成为一名合格的维护人员 / an excellent contributor!

## 维护人员必看系列

向新手村添加一个教程/修改页面需要以下几个步骤：

1. 把新手村所在的 [github 仓库](https://github.com/bit-isp/starter-guide.git) 拷贝到本地
2. 在本地进行预览和修改
3. 把你改好的版本 push 到 [github 仓库](https://github.com/bit-isp/starter-guide.git)

📢 我们来细说这三步要如何执行

### 1. 把仓库拷贝到本地
```bash
git clone https://github.com/bit-isp/starter-guide.git
cd starter-guide
```

### 2. 在本地进行预览和修改

这个网页是用 Hugo 写的，需要先安装 Hugo 来进行本地预览，根据你的操作系统选择安装方式

{{< tabs "uniqueid" >}}
{{< tab "Windows" >}}
# Windows

1. 安装 chocolate
   
    以管理员身份打开 PowerShell, 运行下面这行指令

    ```bash
    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
    ```

2. 用 chocolata 安装 Hugo

    ```bash
    choco install hugo-extended --version==0.88.0
    ```

3. 运行下面这行指令

    ```bash
    hugo server
    ```

    即可通过这个网站进行预览：[http://localhost:1313/starter-guide/](http://localhost:1313/starter-guide/)

{{< /tab >}}


{{< tab "Mac" >}}
# Mac

Pending.
{{< /tab >}}

{{< tab "Linux" >}}

# Linux

Pending.
{{< /tab >}}
{{< /tabs >}}


现在，你应该可以在你自己的浏览器里看到新手村了。
接下来，我们来学习如何添加一个教程/修改页面。

每一个页面都是用 Markdown 语法写的，基本语法可以在[这里](https://markdown.com.cn/basic-syntax/) 找到。

打开你本地的 `starter-guide` 文件夹，只需要修改 `content` 里面的东西。

```
├─content
│  ├─docs             # 这里面是 公共资源、论文写作、其他
│  │  ├─others           # 其他
│  │  ├─share            # 公共资源
│  │  └─writing          # 论文写作
│  └─posts            # 这里面是 博客
```

以添加一篇[介绍 Tmux 的博客](https://bit-isp.github.io/starter-guide/posts/tmux/) 为例，打开 `content/posts`, 新建一个 `tmux.md`, 写入以下内容

```md
---
author: "你的名字"
date: 20xx-xx-xx
title: Tmux 简易教程
---

如果你希望关闭 terminal 窗口后，你的程序仍在服务器端运行，你可以试试 tmux 。（这句话会显示在博客首页）

<!--more-->
```

后面就是按照 Markdown 语法来写你的教程了。


### 3. 把本地版本 push 上去
```bash
git push
```

## 访问数据

{{< visit_count >}}

## 待办事项

- [x] 代码块暗黑模式自动切换 @2022-6-22 ~ @2022-6-22
    - https://bwiggs.com/posts/2021-08-03-hugo-syntax-highlight-dark-light/
- [x] 1080p 字体优化  @2022-6-22 ~ @2022-6-22
    - https://github.com/lxgw/LxgwWenKai
    - https://github.com/chawyehsu/lxgw-wenkai-webfont
- [x] 访问量统计 @2022-6-22 ~ @2022-6-25
- [ ] 评论区 @2022-6-25
- [ ] hugo 教程 
- [ ] Contributor Guide