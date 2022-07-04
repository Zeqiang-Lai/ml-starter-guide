---
title: "Cuda"
---

# Cuda Toolkit

实验室服务器的共享目录包含数个预先安装好的 `Cuda` 版本。

这些共享 Cuda 位于 `/share/opt/` ，包含：

```
cuda-11.3.1
cuda-11.1.0
cuda-10.2
```

## 切换 Cuda 版本

{{< hint warning >}}
**注意** ⚠️ ：大部分情况你应该都不用使用这个, Conda 安装的 PyTorch 自带 Toolkit。

一般来说，只有在你需要编译自定义 Cuda 算子的时候，才可能需要下面的操作，如果你看不懂这里在说什么，那么大概率你不需要以下操作。
{{< /hint >}}


在 `.bashrc` 或 `.zshrc` 中添加以下内容

大部分情况设置这个应该就够了

```shell
export CUDA_HOME=/share/opt/cuda-11.3.1 
```

如果不行，添加

```shell
export LD_LIBRARY_PATH=/share/opt/cuda-11.3.1/lib64:$LD_LIBRARY_PATH
export PATH=/share/opt/cuda-11.3.1/bin:$PATH
```
