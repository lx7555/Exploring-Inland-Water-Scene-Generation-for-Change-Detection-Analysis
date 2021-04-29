# Exploring-Urban-Water-Scene-Generation-for-Change-Detection-Analysis


## Abstract

Change detection is becoming indispensable for unmanned aerial vehicles, especially in 
the domain of water landing, rescue and search. However, even the most advanced change detectors 
require large amounts of data for model training and testing. Therefore, a sufficient variety of 
labeled images with different imaging conditions are needed. In this paper, we present a cloning 
method to simulate water-scene and collect labeled multi-challenge sequences automatically. The multi-challenge sequences consist of six challenges to test the effects of dynamic background, weather, and noise on change detection models. Then, we propose an image-translation framework that translates simulated images to synthetic images. This framework uses shared parameters (encoder and generator) and 10 × 10 receptive fields (discriminator), so it can generate realistic synthetic images as model training sets. The experimental results indicate that: 1) different imaging challenges will affect the performance of change detection models; 2) compared with simulated images, the synthetic images can effectively improve the accuracy of (supervised) change detection models.

## Description
Considering that change detection models have to deal with some challenges of water scenes, we generate various simulated multi-challenge sequences, 
including Basic, Dynamic Background, Illumination Variations, Bad Weather, Video Noise, and More Moving Objects. Note:
Each specific sequence is also affected by other challenges, but one challenge is dominant.
Besides, we propose an image-translation framework that translates simulated images to realistic synthetic images.

## The overall framework of the proposed method
![image](https://github.com/lx7555/Exploring-Urban-Water-Scene-Generation-for-Change-Detection-Analysis/blob/main/image/fig2.jpg)

## Examples of the real, simulated and synthetic dataset
![image](https://github.com/lx7555/Exploring-Urban-Water-Scene-Generation-for-Change-Detection-Analysis/blob/main/image/fig7.jpg)


## Download
Simulated Multi-challenge Sequence is a water-scene dataset designed to design and evaluate a variety of computer vision models for change detection.
We provide one [.rar] archive per type of data as described below. Our indexes always start from 000001. In the following,

Simulated Multi-challenge Sequences_rgb_2021: Each area is simply a folder in the format: The compressed file contains the original image.

[Simulated Multi-challenge Sequence_rgb_2021.rar](https://drive.google.com/file/d/1Bpjgt9N87UX-U8n6vtHOVwxVkoJpbquK/view?usp=sharing)

Simulated Multi-challenge Sequences_gt_2021: The compressed file contains the ground truth of object detection. The per-pixel segmentation ground truth is encoded as per-frame .png files (standard 8-bit precision per channel).

[Simulated Multi-challenge Sequence_gt_2021.rar](https://drive.google.com/file/d/16ZCpV8VFezS0aaH7uIozPOYaPtj5KpfK/view?usp=sharing)

## Sample images of simulated multi-challenge sequences
![image](https://github.com/lx7555/Exploring-Urban-Water-Scene-Generation-for-Change-Detection-Analysis/blob/main/image/fig4.jpg)

## Examples of change detection results on simulated multi-challenge sequences using different models
![image](https://github.com/lx7555/Exploring-Urban-Water-Scene-Generation-for-Change-Detection-Analysis/blob/main/image/fig9.jpg)

## Citations
All rights of the Simulated Multi-challenge and Synthetic Dataset are reversed by the Peng Cheng Laboratory. It is free for academic research, and your cooperation with us is appreciated. Feel free to contact us if you have any questions.

If the Synthetic-Boat-Sequence Dataset is used in your research, please cite the following papers:

1. Xuan Li, Kunfeng Wang, Yonglin Tian, Lan Yan, Fang Deng, Fei-Yue Wang, "The ParallelEye Dataset: A Large Collection of Virtual Images for Traffic Vision Research," 
IEEE Transactions on Intelligent Transportation Systems, 2018, 20(6): 2072-2084. [Link](https://ieeexplore.ieee.org/document/8451919/)

2. Xuan Li, Yutong Wang, Lan Yan, Kunfeng Wang, Fang Deng, Fei-Yue Wang, "ParallelEye-CS: A New Dataset of Synthetic Images for Testing the Visual Intelligence of Intelligent Vehicles," IEEE Transactions on Vehicular Technology, 2019, 68(10): 9619-9631. [Link](https://ieeexplore.ieee.org/abstract/document/8807212)

3. Xuan Li, Kunfeng Wang, Xianfeng Gu, Fang Deng, Fei-Yue Wang, "ParallelEye Pipeline: An Effective Method to Synthesize Images for Improving the Visual
Intelligence of Intelligent Vehicles," IEEE Transactions on Systems Man Cybernetics-Systems.(accepted) 


