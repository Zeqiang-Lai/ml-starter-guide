---
author: "村民1号"
date: 2022-06-20
title: Conda 简易教程
---


<!--more-->

## 基础用法

- 查看当前环境安装了哪些包

```shell
conda list
```

- 查看当前存在哪些虚拟环境

```shell
conda env list
```


- 创建虚拟环境

```shell
conda create -n your_env_name python=X.X
```

如果你想把环境装到别的指定文件夹里, 用 `-p` 而不是 `-n` 然后指定完成路径。
```shell
conda create -p full_path python=X.X
```

- 删除虚拟环境

```shell
conda env remove -n name
```

## 环境拷贝

- 环境拷贝可以省去安装下载时间，直接从已有环境复制一份。
- 推荐在使用公共环境的时候，使用环境拷贝复制一个副本，这样就可以随意安装新的package而不会影响到他人。
- 部分pip安装的包可能需要重新下载，但大部分包都是直接复制的。

```shell
conda create -n [name] --clone [path]
```

