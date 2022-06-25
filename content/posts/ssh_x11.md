---
author: "村民1号"
date: 2022-06-25
title: "SSH远程显示Matplotlib等图形界面"
---

通过本教程，你将可以在本地机器显示远程机器上运行 `plt.show()` 显示的窗口。

<!--more-->

## 效果

- VSCode

![demo.gif](demo.gif)

- 命令行需要额外操作：
  - macos 需要给SSH加 `-X`  参数（大写X），例如 `ssh -X user@10.10.10.8`
  - windows下需要用支持x11 forward的terminal，比如xshell，tabby terminal，在profile里找到x11 forward勾上，例如tabby：

![tabby](tabby.png)

![2.gif](2.gif)

其他GUI软件也是可以显示的，比如 `gedit` , `pycharm` 等

![3.gif](3.gif)

## 1. 安装软件

{{< tabs "uniqueid" >}}
{{< tab "macOS" >}}

- 安装xquartz , 地址 https://www.xquartz.org/

{{< /tab >}}

{{< tab "Windows" >}}

- 安装Xming, 地址 [https://sourceforge.net/projects/xming/](https://sourceforge.net/projects/xming/)

{{< /tab >}}
{{< /tabs >}}

## 2. VSCode 配置

- vscode 安装remote x11插件
  - 本地装Remote x11 ssh
  - 远程装Remote x11

![Untitled](x11.png)

![Untitled](x11-2.png)

## 3. 配置`~/.ssh/config`

![Untitled](ssh.png)

- 改`~/.ssh/config`，在你要远程的Host添加 `ForwardX11 yes`

```config
Host 3090-Local
  HostName 10.108.10.37
  User laizeqiang
  ForwardX11 yes
```

## 4. 测试

```python
import matplotlib.pyplot as plt; import numpy as np; img = np.ones((10,10)); plt.imshow(img); plt.show()
```
