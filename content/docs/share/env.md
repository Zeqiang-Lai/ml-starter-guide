---
title: "Conda环境"
weight: 3
---

# 公用 Conda 环境

## 公共环境列表

| 环境路径           | Python版本 | PyTorch版本 | CUDA版本 |
| ------------------ | ---------- | ----------- | -------- |
| /share/envs/qrnn3d | 3.6        | 1.10         | 11.3     |


## 使用方法

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

