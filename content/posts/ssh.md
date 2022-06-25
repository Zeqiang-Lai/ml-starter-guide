---
author: "村民1号"
date: 2022-06-25
title: SSH 免密登陆
---

本文将介绍如何在 Windows 和 macOS 系统配置 SSH 免密登陆。

<!--more-->

## 1.客户端生成公私钥

本地客户端生成公私钥：（一路回车默认即可）

```shell
ssh-keygen
```

上面这个命令会在用户目录.ssh文件夹下创建公私钥

```shell
cd ~/.ssh
ls
```

你会看到以下两个文件：

```txt
1. id_rsa （私钥）
2. id_rsa.pub (公钥)
```

## 2.上传公钥到服务器

假设这里测试用的服务器地址为：192.168.235.22，用户为：root

{{< tabs "uniqueid" >}}
{{< tab "macOS" >}}

macOS 用户可以使用以下命令上传公钥

```shell
ssh-copy-id -i ~/.ssh/id_rsa.pub root@192.168.235.22
```

{{< /tab >}}

{{< tab "Windows" >}}

Windows 用户可以用 [git bash]({{< relref "posts/git" >}})，键入以下命令即可上传

```shell
cat ~/.ssh/id_rsa.pub | ssh laizeqiang@10.140.0.32 "cat >> ~/.ssh/authorized_keys"
```

{{< /tab >}}
{{< /tabs >}}

**解释**

- 上面这条命令实际是将 `~/.ssh/id_rsa.pub` 附加到服务器上的 `~/.ssh/authorized_keys` 文件中。

```shell
cd ~/.ssh
vim authorized_keys
```

通过上述指令，可以看到客户端写入到服务器的 id_rsa.pub （公钥）内容。

## 3.测试免密登录

客户端通过ssh连接远程服务器，就可以免密登录了。

```shell
ssh root@192.168.235.22
```
