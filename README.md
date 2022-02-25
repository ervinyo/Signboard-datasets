# Signboard Datasets

<p align="center">Domain Adaptation Deep Attention Network for Automatic Logo Detection and Recognition in Google Street View</p>
<p align="center">Ervin Yohannes, Chih-Yang Lin, Timothy K. Shih, Chen-Ya Hong, Avirmed Enkhbat, Fitri Utaminingrum</p>
<br>
<!--
<p align="center">Department of Computer Science and Information Engineering, National Central University, Taoyuan City 32001, Taiwan</p>
<p align="center">Department of Electrical Engineering, Yuan-Ze University, Taoyuan City 32003, Taiwan</p>
<p align="center">Faculty of Computer Science, University of Brawijaya, Malang City 65145, Indonesia</p>
-->
<img src="drawing1.png">


# Abstract

<p style="text-align:justify"> Signboards are important location landmarks that provide services to a local community. They are difficult to detect and recognize due to the myriad of designs that combine text and images. Many people only see signboards as sign of place and attract attention of them. However, the impaired visually people can’t see like the usual people about signboards. They need an assistance system to guided them go to destination. Currently, the assistance system still remaining issue since limited datasets to create the best one and also need long computation time for reaches the best results. In this paper, we propose a novel framework that can automatically detect and recognize signboard logos. In addition, we utilizing Google street view for collecting our datasets in around Taiwan’s street. This framework consists of a domain adaptation that not only reduces the loss function between source-target datasets but also represents important source features adopted by the target dataset and deep learning techniques for the detection and recognition system. In our model, we add nonlocal blocks and attention mechanisms called deep attention networks to achieve the best final result. We perform extensive experiments on both our and public datasets to show superior performance and effectiveness of our proposed method. The experimental results show our proposed method outperform the baseline in all evaluation metrics of state-of-the-art detection and recognition method.</p>


# Overview
our dataset is a signboard dataset containing 29,727 images with VOC annotation format and a resolution of 500 × 400 pixels. Our dataset consists of 14 classes of store logos, including Carrefour, Domino, Family Mart, Gas, Hi-Life, KFC, McDonald, Mos Burger, Ok Mart, Post, Pxmart, 7-ELEVEN, Starbucks, and Wellcome. We already divided our datasets into training and validation.

<img src="img2.png">

# Requirements
1. install anaconda and python 3.6.10 <a href="https://drive.google.com/drive/folders/1tElCRmh5O18gq_iTTMrTlSwgH1zvJKmV?usp=sharing">See Here</a>
2. setting environment variable which using CUDAv10.0 and cudnn64_7(put in bin(.dll), include(.h), and lib x64(.lib))<a href="https://drive.google.com/drive/folders/1tElCRmh5O18gq_iTTMrTlSwgH1zvJKmV?usp=sharing">Download Here</a>
3. install tensorflow-gpu=1.14.0
4. install keras=2.2.4

# Download
The link for download the datasets and annotations as follow :

<a href="https://drive.google.com/drive/folders/1tElCRmh5O18gq_iTTMrTlSwgH1zvJKmV?usp=sharing">Download Datasets</a>

# Results

The comparison results for SSD, YOLOv2, YOLOv3, YOLOv4, and our proposed method are shown in below
<table style="width:100%">
  <tr>
    <th>SSD</th>
    <th>YOLOv2</th>
    <th>YOLOv3</th>
    <th>YOLOv4</th>
    <th>Our proposed method I</th>
    <th>Our proposed method II</th>
  </tr>
  <tr>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/7-11/SSDs.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/7-11/YOLOv2s.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/7-11/YOLOv3s.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/7-11/YOLOv4s.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/7-11/propose1s.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/7-11/propose2s.png"></td>
  </tr>
  <tr>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Hi Life/SSDh.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Hi Life/YOLOv2h.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Hi Life/YOLOv3h.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Hi Life/YOLOv4h.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Hi Life/propose1h.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Hi Life/propose2h.png"></td>
  </tr>
  <tr>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/OkMart/SSDo.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/OkMart/YOLOv2o.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/OkMart/YOLOv3o.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/OkMart/YOLOv4o.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/OkMart/propose1o.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/OkMart/propose2o.png"></td>
  </tr>
  <tr>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Family Mart/SSDf.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Family Mart/YOLOv2f.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Family Mart/YOLOv3f.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Family Mart/YOLOv4f.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Family Mart/propose1f.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/Family Mart/propose2f.png"></td>
  </tr>
  <!-- Write your comments here 
  <tr>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/BSVSO/SSD64.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/BSVSO/YOLOv264.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/BSVSO/YOLOv364.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/BSVSO/YOLOv464.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/BSVSO/propose164.png"></td>
    <td><img src="https://github.com/ervinyo/Signboard-datasets/blob/main/Results/BSVSO/propose264.png"></td>
  </tr>
  -->
</table>

# Citation
If you use this dataset in your research, please include the following citation in any published results.
```
@ARTICLE{9491158,
author={Yohannes, Ervin and Lin, Chih-Yang and Shih, Timothy K. and Hong, Chen-Ya and Enkhbat, Avirmed and Utaminingrum, Fitri},  
journal={IEEE Access},  
title={Domain Adaptation Deep Attention Network for Automatic Logo Detection and Recognition in Google Street View},  
year={2021},  
volume={9},
number={}, 
pages={102623-102635}, 
doi={10.1109/ACCESS.2021.3098713}}
```
