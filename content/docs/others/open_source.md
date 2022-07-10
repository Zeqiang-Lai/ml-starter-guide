---
title: "开源规范"
---

# 开源规范

作者: chengshuang

1. 没有上传代码的同学请尽快上传
2. 已上传代码的同学请检查其中是否有失效链接（百度网盘，onedrive）

另外，请大家按照以下模板中的内容对readme内容进行统一。

## README模版

{{< button href="../readme_template" >}}模版预览{{< /button >}}

{{< highlight markdown >}}

# Method name

[Paper](link) | [Pretrained Model](link)

**Title (CVPR 2021)**

Author1, Author2, Author3

## News [optional]

## Introduction

paper的abstract

## Highlights

+ 创新点1
+ 创新点2
+ 创新点3

## Network Architecture

附图

## Result

附图

## Requirement

- Pytorch >= 1.8
- OpenCV
- ......

## Getting Started

（可参考以下内容）

1.  **Install the requirments**

```shell
conda install -c conda-forge opencv
conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch
pip install -r requirements.txt
```

2. **Clone the repo**

```shell
git clone https://github.com/Zeqiang-Lai/DPHSIR.git
cd DPHSIR
pip install -e .
```

3. **Run cli or playgrounds**

- Download the [sample input](https://1drv.ms/u/s!AomvdxwcLmYImEc-Yfj2B2FBGEb0?e=vShXe9) if you don't have one.

```shell
# run cli
python cli/main.py -i [input_path] [task]
# run playground
python playgrounds/deblur.py
```

## Citation

If you find this work useful for your research, please cite:

```bibtex
Bibtex
```

## Acknowledgement [optional]
{{< /highlight >}}

