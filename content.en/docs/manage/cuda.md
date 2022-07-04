# CUDA 管理

{{< hint warning >}}
此部分内容极其容易引起错误导致训练环境崩溃，请谨慎操作。
{{< /hint >}}

目前安装有的共享 Cuda 位于 `/share/opt/` ，包含：
```
cuda-11.3.1
```

## 多版本 CUDA 管理

前往 [官网](https://developer.nvidia.com/cuda-toolkit-archive) 下载需要版本的 Cuda Toolkit。

选 `run_file(local)` 这个版本。

{{< figure src="../imgs/cuda.png" >}}

下载完毕后，运行以下命令：
```
sudo sh cuda-9.1.run --silent --toolkit --toolkitpath=/share/opt/cuda-9.1
```

参数：
- `--toolkit`: **重要参数！！！**，只安装 toolkit，不装显卡驱动。**一定要包含这个**。
- `--silent`: 静默安装，不会显示过程。
- `--toolkitpath`: 指定安装地址。


## 多版本 CUDA 切换

在 `.bashrc` 或 `.zshrc` 中添加以下内容

大部分情况设置这个应该就够了

```
export CUDA_HOME=/share/opt/cuda-11.3.1 
```

如果不行，添加

```
export LD_LIBRARY_PATH=/share/opt/cuda-11.3.1/lib64:$LD_LIBRARY_PATH
export PATH=/share/opt/cuda-11.3.1/bin:$PATH
```


## 参考资料

- https://notesbyair.github.io/blog/cs/2020-05-26-installing-multiple-versions-of-cuda-cudnn/
- https://blog.kovalevskyi.com/multiple-version-of-cuda-libraries-on-the-same-machine-b9502d50ae77



