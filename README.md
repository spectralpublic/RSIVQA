# RSIVQA (Remote Sensing Image Visual Question Answering)
RSIVQA is a remote sensing visual question answering dataset proposed in the paper "Mutual Attention Inception Network for Remote Sensing Visual Question Answering".
If this data set is used in your work, please cite our paper.

[1] X. Zheng, B. Wang, X. Du, and X. Lu, “Mutual Attention Inception Network for Remote Sensing Visual Question Answering,” IEEE Transactions on Geoscience Remote Sensing, 2021.

@article{
9444570,
author = {Zheng, Xiangtao and Wang, Binqiang and Du, Xingqian and Lu, Xiaoqiang},
doi = {10.1109/TGRS.2021.3079918},
issn = {0196-2892},
journal = {IEEE Transactions on Geoscience and Remote Sensing},
title = {{Mutual Attention Inception Network for Remote Sensing Visual Question Answering}},
year = {2021}
}

## Overview

RSIVQA dataset is derived from existing *remote sensing image* (RSI) datasets with a specially designed generation method.   

Currently, images of RSIVQA come from three RSI classification datasets 
([UCM](http://weegee.vision.ucmerced.edu/datasets/landuse.html), Sydney and 
[AID](https://pan.baidu.com/s/1mifOBv6#list/path=%2F)) and two RSI object detection datasets 
([HRRSD](https://github.com/CrazyStoneonRoad/TGRS-HRRSD-Dataset) and 
[DOTA](https://captain-whu.github.io/DOTA/index.html)). Questions and answers are generated based on 
images to form image-question-answer triplets. Questions, answers and their correspondence can 
be found in txt files in this repository. Images of the datasets can be downloaded from the link of 
each dataset.

## Deatails
There are ***37264 images*** and ***111134 image-question-answer triplets*** in the dataset. Detaled information is summarized in the table below.  

| Item                                 | Amount |
|--------------------------------------|:------:|
| The number of images                 |  37264 |
| The number of unique questions       |   91   |
| The number of unique answers         |   574  |
| The total number of VQA triplets     | 111134 |
| The number of yes or no VQA triplets |  64610 |
| The number of number VQA triplets    |  32331 |
| The number of others VQA triplets    |  14193 |

A small part of RSIVQA is annotated by human. Others are automatically generated using existing scene classification datasets and object detection datasets. For more detailed information of the generation method, please refer to the paper.  

## Files

The question and answers are saved in txt files. Each line includes an IQA triplet and three parts are seprated by colon and question mark.  
For example, in sydney_vqa.txt, the first line is
>1.tif:what is the theme of this picture?residential  

which means the question for the image "1.tif" is "what is the theme of this picture?". The answer for the question is "residential". "1.tif" is file name of the image.  

Image-question-answer triplets for each origin scene classification or object detection dataset are saved in corresponding folders.

--------------------------------------
To be finished....
