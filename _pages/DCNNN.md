---
title: "Enliten Lab - DCNNN"
layout: textlay
excerpt: "Enliten Lab -- DCNNN"
sitemap: false
permalink: /research/DCNNN/
---

# DCNNN [(back)](https://enliten.utk.edu/research/)

## DCNNN Toolbox for Contingency Screening with 100x Acceleration 

![]({{ site.url }}{{ site.baseurl }}/images/respic/DCNNN_toolbox.jpg){: style="width: 600px; float: center; border: 10px"}

The main idea behind DCNNN is to train a deep CNN for classifying system security status as well as obtaining system state parameters. Fig. 1. explains how the DCNNN toolbox works for fast contingency screening. Given a power system, the bus active/reactive power injection, and the bus self-susceptance elements are selected as the input to deep CNN. The deep CNN consists of two convolutional (Conv) layers and three fully-connected (FC) layer. The function of the convolutional layers is to extract features from the input power system raw data. The function of the fully-connected layer is to map the extracted features to the desired output.

There are two types of output from deep CNN: the first is a matrix containing bus voltage magnitude and bus voltage angle; the second is the system security status. It can be observed that the proposed deep CNN can realize two functions simultaneously: as an AC power flow (ACPF) regression tool to get system state parameters and as a classifier for system security assessment under N-1 contingency, which is a multi-task learning model. The system security status evaluates the system as whole, while the bus voltage can reflect the local vulnerability.

![]({{ site.url }}{{ site.baseurl }}/images/respic/DCNNNstructure.jpg){: style="width: 1000px; float: center; border: 10px"}

To validate the efficiency and accuracy of DCNNN, we compare the screening results and the calculation time from DCNNN with that of the model-based ACPF method, as shown in the following tables.

In Table 1, the errors of sita and v are the per unit mean absolute value over the test set compared with the results from model-based ACPF calculation. The classification accuracy is the ratio between the number of test samples that have been correctly classified based on their security status and the total number of test samples. As the table shows, DCNNN model possesses considerably high accuracy for ACPF calculation, even for large-scale power systems. Also, the training time is within an acceptable range given that the training is completed off-line.

![]({{ site.url }}{{ site.baseurl }}/images/respic/DCNNNtable1.png){: style="width: 500px; float: center; border: 10px"}

In Table 2, the last column shows the acceleration based on the computing time of DCNNN and the model-based ACPF method. The DCNNN approach is from 129 to 240 times faster than the latter, with an average of 205 times faster. This is because the well-trained DCNNN has high generalization to unseen test cases, and it can automatically generate AC power flow results and classify system security status under the new given input without iterative calculation of power flows.

![]({{ site.url }}{{ site.baseurl }}/images/respic/DCNNNtable2.png){: style="width: 400px; float: center; border: 10px"}

Useful links:
  
· [DCNNN User Manual]({{ site.url }}{{ site.baseurl }}/downloads/DCNNN_User_Manual.pdf)
  
· [A short letter for deep CNN-based contingency screening：](https://ieeexplore.ieee.org/abstract/document/8705389) Yan Du, Fangxing Li, Jiang Li, and Tongxin Zheng, "Achieving 100x Acceleration for N-1 Contingency Screening with Uncertain Scenarios using Deep Convolutional Neural Network," IEEE Transactions on Power Systems, vol. 34, no. 4, pp. 3303-3305, July 2019.
  
· [A full paper for cascading outage screening using deep CNN and depth-first search algorithm：](https://ieeexplore.ieee.org/abstract/document/8972476) Yan Du, Fangxing Li, Tongxin Zheng, Jiang Li, "Fast Cascading Outage Screening based on Deep Convolutional Neural Network and Depth-First Search," IEEE Transactions on Power Systems, vol. 35, no. 4, pp. 2704-2715, July 2020.


Contact Info:  Dr. Fangxing(Fran) Li, University of Tennessee, Knoxville, fli6@utk.edu, 865-974-8401
