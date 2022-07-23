---
title: "高光谱图像分类"
weight: 1
---

# 高光谱图像分类数据集

## 1 Indian Pines
Indian Pines由AVIRIS传感器在印第安纳州西北部的试验场上空采集。图像大小为145*145像素，包含220个波段，波段范围为0.4-2.5 (10^-6m)。

数据来源：[Indian Pines](https://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes)

本地路径：**/share/dataset/hsi_classification/Indian Pines**

![Indian Pines Ground Truth](../imgs/hsi_classification/Indian_Pines.png)

**Ground Truth**
|#|Class|Samples|
|:---:|:---:|:---:|
|1|Alfalfa|	46|
|2|Corn-notill|	1428|
|3|Corn-mintill|	830|
|4|Corn	|237|
|5|Grass-pasture	|483|
|6|Grass-trees	|730|
|7|Grass-pasture-mowed	|28|
|8|Hay-windrowed	|478|
|9|Oats	|20|
|10|Soybean-notill	|972|
|11|Soybean-mintill	|2455|
|12|Soybean-clean	|593|
|13|Wheat	|205|
|14|Woods	|1265|
|15|Buildings-Grass-Trees-Drives	|386|
|16|Stone-Steel-Towers	|93|

## 2 Salinas
该场景由加利福尼亚州萨利纳斯山谷的224波段AVIRIS传感器采集，具有高空间分辨率（3.7米像素）的特点。图像大小为512*217，包含224个波段。

数据来源：[Salinas](https://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes)

本地路径：**/share/dataset/hsi_classification/Salinas**

![Salinas](../imgs/hsi_classification/Salinas.png)

**Ground Truth**
|#|Class|Samples|
|:---:|:---:|:---:|
|1|Brocoli_green_weeds_1	|2009|
|2|Brocoli_green_weeds_2	|3726|
|3|Fallow	|1976|
|4|Fallow_rough_plow	|1394|
|5|Fallow_smooth	|2678|
|6|Stubble	|3959|
|7|Celery	|3579|
|8|Grapes_untrained	1|1271|
|9|Soil_vinyard_develop	|6203|
|10|Corn_senesced_green_weeds	|3278|
|11|Lettuce_romaine_4wk	|1068|
|12|Lettuce_romaine_5wk	|1927|
|13|Lettuce_romaine_6wk |916|
|14|Lettuce_romaine_7wk	|1070|
|15|Vinyard_untrained	|7268|
|16|Vinyard_vertical_trellis	|1807|

## 3 Pavia Center and University
Pavia Center和Pavia University数据集由ROSIS传感器在意大利Pavia城市上空采集。

数据来源：[Pavia](https://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes)

本地路径：**/share/dataset/hsi_classification/Pavia**


### 3.1 Pavia Center sence
Pavia Center图像大小为1096*715，包含102个波段。

![Pavia Center](../imgs/hsi_classification/Pavia_Center.png)

**Ground Truth**
|#|	Class	Samples|
|:---:|:---:|:---:|
|1|	Water	|824|
|2|	Trees	|820|
|3|	Asphalt	|816|
|4|	Self-Blocking Bricks	|808|
|5|	Bitumen	|808|
|6|	Tiles	1|260|
|7|	Shadows	|476|
|8|	Meadows	|824|
|9|	Bare Soil	|820|

Pavia Center图像大小为1096*715，包含102个波段。

### 3.2 Pavia Unitersity sence
Pavia Unitersity sence图像大小为610*340，包含103个波段。


![Pavia University](../imgs/hsi_classification/Pavia_University.png)


|#|	Class	Samples|
|:---:|:---:|:---:|
|1|	Asphalt|	6631
|2|	Meadows	|18649
|3|	Gravel|	2099
|4|	Trees|	3064
|5|	Painted metal sheets|	1345
|6|	Bare Soil|	5029
|7|	Bitumen|	1330
|8|	Self-Blocking Bricks|	3682
|9|	Shadows|	947

## 4 Kennedy Space Center(KSC)
Kennedy数据集由AVIRIS传感器在美国佛罗里达州肯尼迪航天中心获取数据。图像大小为512*614，包含176个波段

数据来源：[Kennedy](https://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes)

本地路径：**/share/dataset/hsi_classification/Kennedy_Space_Center**

![Kennedy Space Center](../imgs/hsi_classification/Kennedy_Space_Center.gif)

## 5 Wuhan_UAV-borne_hyperspectral_image
WuHan_Hi数据集由Headwall Nano-Hyperspec传感器采集。包含LongKou(龙口)、HanChuan(汉川)、HongHu(洪湖)三个数据集。

数据来源：[武汉大学——智能化遥感数据提取分析与应用研究组](http://rsidea.whu.edu.cn/resource_WHUHi_sharing.htm)

### 5.1 WHU-Hi-HanChuan
HanChuan图像大小为1217*303，包含274个波段

### 5.2 WHU-Hi-HongHu
HongHu图像大小为940*475，包含270个波段

### 5.3 WHU-Hi-LongKou
LongKou图像大小为550*400，包含270个波段
