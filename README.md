# ML Starter Guide

```shell
git clone --recursive https://github.com/Zeqiang-Lai/ml-starter-guide.git
git submodule update --init --recursive
```

你需要使用 [0.88](https://github.com/gohugoio/hugo/releases/tag/v0.88.1) **Extened** 版本的 Hugo，否则会报错。

Linux 安装

```shell
sudo dpkg -i hugo_extended_0.88.1_Linux-64bit.deb
```


实时预览

```shell
hugo server
```

Github Action

已经配好了, push 就会自动部署到 Github Pages 。

## Reference

-  https://github.com/peaceiris/actions-hugo