---
author: "赖泽强"
date: 2022-06-20
title: 如何配置趁手的命令行环境
---

如果你的命令行 shell 是 bash，你可以跟随这个教程配置更好用的 zsh 。

<!--more-->

## Introduction

如何查看自己的 shell 的类型？

请在命令行键入以下命令

```shell
echo $SHELL
```

## 效果

你的命令行将支持

1. 语法高亮
2. git 提示
3. 自动补全
4. 更棒的历史记录
5. 等

示意

![example](example.gif)


## 方法

1. 设置默认 shell 为 zsh

```shell
chsh -s /bin/zsh
```

2. 进入 zsh

```shell
zsh
```

第一次使用会弹出是否新建配置文件，选 `populate .zshrc`

3. 配置 `oh my zsh` 

```shell
sh -c "$(wget https://gitee.com/Devkings/oh_my_zsh_install/raw/master/install.sh -O -)"
```

4. 配置高亮，自动补全插件

先执行这两

```shell
git clone https://gitee.com/han8gui/zsh-autosuggestions.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://gitee.com/Annihilater/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

然后修改配置文件

```shell
vim ~/.zshrc
```

找到如下这行配置代码，在后面追加插件名
```
plugins=(zsh-autosuggestions zsh-syntax-highlighting)
```

## 更多阅读

- [oh my zsh](https://ohmyz.sh/)
