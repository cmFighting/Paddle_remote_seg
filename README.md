# 飞桨常规赛：遥感影像地块分割- 9月第3名方案

## 项目描述

本次的飞桨常规赛主要是对遥感影像进行像素级内容解析，并对遥感影像中感兴趣的类别进行提取和分类，以衡量遥感影像地块分割模型在多个类别（如建筑、道路、林地等）上的效果。

我采用的方案是deeplabv3+, 并使用了diceloss替换了原先的celoss, 在GPU的环境下训练了8个小时左右得到的50.316的精度。

最优模型下载地址：

> 链接：https://pan.baidu.com/s/1inr2nRJAn1CvZqDSPuoIFA 
> 提取码：rx0w 

## 项目结构

本项目借助paddle的[PaddlePaddle/PaddleSeg: End-to-end image segmentation kit based on PaddlePaddle. (github.com)](https://github.com/PaddlePaddle/PaddleSeg)进行实现，主要使用到的文件以及文件夹如下：

```
-|configs # 配置文件
-|paddleseg # paddleseg框架
-README.MD # 本文件
-run.ipynb # 训练、测试运行脚本文件 
```

## 使用方式

你可以在AI Studio上[飞桨常规赛：遥感影像地块分割 - 9月第3名方案 - 飞桨AI Studio - 人工智能学习实训社区 (baidu.com)](https://aistudio.baidu.com/aistudio/projectdetail/2479183)，百度每天会送你8点算力卡，可以使用16个小时的v100显卡，非常nice，fork本项目之后直接启动即可快速完成整个训练和测试的过程。

