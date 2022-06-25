---
author: "🍉"
date: 2022-06-20
title: Tmux 简易教程
---

如果你希望关闭 terminal 窗口后，你的程序仍在服务器端运行，你可以试试 tmux 。

<!--more-->

## 介绍

一般来说，我们都是用自己电脑上的 vscode/pycharm 连接远程服务器跑实验。如果直接在 terminal 里输入指令，让程序运行起来，我们就不能退出 vscode/pycharm, 因为程序会终止。此外，自己电脑意外断网也会导致断连，程序终止。

Tmux 就是一个在我们关闭了终端窗口再打开，会话并不终止，而是继续运行之前程序的工具。


## 效果
![example](tmux_01.gif)


## 使用

首先，我们了解一下 **会话** 和 **窗口** 两个概念。

以做实验为例，假设我们需要在两个数据集（dataset_A, dataset_B）上跑两个实验（baseline, ours），我们可以开两个**会话**、起名为dataset_A和dataset_B；然后我们在dataset_A中新建两个**窗口**、起名为baseline和ours, 在这两个窗口中分别跑baseline和ours的实验。同样地，在dataset_B这个会话中，我们也新建baseline和ours两个窗口，跑dataset_B下的实验。

1. 新建会话

```shell
tmux                               # 默认从0开始命名
tmux new -s 会话名 -n 窗口名
```

2. 列出全部的会话
```shell
tmux ls
```

3. 恢复会话
```shell
tmux at -t 会话名
```

4. 删除会话
```shell
tmux kill-session -t 会话名
```
