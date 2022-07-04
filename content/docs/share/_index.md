---
weight: 1
bookFlatSection: true
title: "公共资源"
---

# 公共资源

实验室的服务器设置有**公共数据集**，**公共Conda环境**，**公共软件资源**等。

大家可以按需自行获取使用。

## 存放位置

| 内容          | 路径            |
| ------------- | --------------- |
| 公共数据集    | /share/dataset  |
| 公共Conda环境 | /share/envs     |
| 公共软件资源  | /share/software |
| Cuda,GCC等    | /share/opt      |


## 使用方法

**数据集**

1. 大家可以自行读取，但请不要往`/share/dataset`写，以及删除东西（虽然你可能根本没有权限）。
2. 使用 [torchlight]() 里的 `data.dataset` 模块进行读取。（正在实现当中）


**Conda环境**

1. 查看有哪些环境

```shell
ls /share/env
```

2. 激活环境，以 `qrnn3d` 为例，（如果出错了，你可能需要先安装 `conda`）

```shell
source activate /share/envs/qrnn3d
```

{{< hint warning >}}

为方便大家使用，`/share/env` 里的环境没有设置权限。因此

1. 大家可以进行 `pip install` 操作，**禁止** `uninstall` 和 `upgrade` 。
2. 但是，`conda install` 是**不允许**的。（主要考虑是容易破坏包的版本依赖）

{{< /hint >}}

