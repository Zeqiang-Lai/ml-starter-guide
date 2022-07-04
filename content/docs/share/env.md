---
title: "Conda"
weight: 3
---

# 公用 Conda 环境

实验室服务器配置有公共的 `Conda` 环境，大家可以自行 `clone` 或者直接使用

## 公共环境列表

| 环境路径              | Python版本 | PyTorch版本 | CUDA版本 |
| --------------------- | ---------- | ----------- | -------- |
| /share/envs/torch1.7  | 3.6        | 1.7.1         | 11.0     |
| /share/envs/torch1.10 | 3.7        | 1.10.0        | 11.3.1     |


## 使用方法

1. 查看有哪些环境

```shell
ls /share/envs
```

### clone

推荐 `clone` 一份到自己的 `home` 目录下，这样可以随意更改，不会影响到他人。

`clone` 使用的是直接复制，所以无需重新下载大部分内容。（部分内容需要下载是正常的）

```shell
conda create -n [name] --clone [path]
```

其中 `[name]` 是你想要的环境名，`[path]` 是你想要的拷贝的环境路径, 例如 `/share/envs/torch1.7`。

详见[Conda教程]({{< relref "posts/conda" >}})

### 直接使用

1. 激活环境，以 `torch1.7` 为例

```shell
conda activate /share/envs/torch1.7
```

{{< hint warning >}}

为方便大家使用，`/share/envs` 里的环境没有设置权限。因此

1. 大家可以进行 `pip install` 操作，**禁止** `uninstall` 和 `upgrade` 。
2. 但是，`conda install` 是**不允许**的。（主要考虑是容易破坏包的版本依赖）

{{< /hint >}}

