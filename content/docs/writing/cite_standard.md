---
author: "lihesong"
date: 2022-07-10
title: 引用规范
---

# 论文引用规范

标准引用格式就是写国际期刊的英文论文时引用别人论文的格式。

到谷歌学术或谷歌学术镜像网站搜论文名，在引用里选BibTex打开。

{{< figure src="img1.png" >}}
{{< figure src="img2.png" >}}


## 会议论文

上面这个例子里第一行@后面是inproceedings，表示是会议论文，标准引用格式为：

[作者1名 姓], [作者2名 姓], and [作者3名 姓]. [论文名]. In [会议全称斜体], pages [起始页码]--[结束页码], [年份]. 

根据上图的BibTeX，该论文应该写成:


> Yunhao Zou, Yinqiang Zheng, Tsuyoshi Takatani, and Ying Fu. Learning to reconstruct high speed and high dynamic range videos from events. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, pages 2024--2033, 2021.


**注意**每个印文标点后都有一个英文空格，页码之间的连接符是两个减号组成的。下面是其它一些会议的引用例子：（下图红色的数字是期刊自动补的页码，不用管）


## 期刊论文

## 预印版论文


## 其它注意事项：

1. 写论文时一般用LaTex，只需把所有要引用的论文的BibTeX放一起，LaTex会自动生成参考文献的标准格式。有些期刊的LaTex模板可能会对标准格式做一点修改，比如名字缩写，咱们一定要提供标准格式的完整版的BibTeX，不要自己做这些改动，要让期刊模板自动改。
1. 如果谷歌学术的BibTex信息不全可以点链接到对应的期刊官方网站，找到“Cite”按钮，查看BibTex引用信息。
2. 期刊的编号（number）如果实在找不到就不写卷号后的括号。
3. 个别期刊的页码可能不是“多少到多少”的形式，而是一长串带字母的编号，就以其期刊官网查到的这个编号为准。
4. 人名有两种表示方法，一种是“名 姓”，一种是“姓, 名”。标准引用格式用的是第一种，因为要和两个人名之间的逗号区分开。
