---
title: Introduction
type: docs
---

# 简介

🌟 欢迎来到新手村。

1. 这里汇总了实验室服务器相关的各种资源使用方法与教程。
2. 常用软件推荐, 各种开发流程优化教程等等。


{{< recent_posts >}}


## 常用指令

切换 pip 源

```shell
pip config set global.index-url https://mirrors.aliyun.com/pypi/simple/
```

训练

```shell
nvidia-smi
export CUDA_VISIBLE_DEVICES=1
source activate /share/envs/qrnn3d
```

Linux 常用命令

```shell
du -sh path # 查看文件大小
ls -sh # 查看文件夹下的文件,并显示大小
df -h # 查看磁盘占用空间
ps -f -p pid # 查看进程是谁运行的
```


## 友情链接

来自[村民一号](https://github.com/Zeqiang-Lai):
- [常用软件使用指南](https://laizeqiang.notion.site/Software-f61bbdd56c324639900872ed175b214f)
- [机器学习基础知识](https://laizeqiang.notion.site/Cheatsheet-2ac821b162fa4196986f368d39953474)
- [torchlight](https://github.com/Zeqiang-Lai/torchlight)


## 贡献

- 欢迎贡献文档，欢迎提出意见和建议。