---
title: "Enliten Lab - Research"
layout: textlay
excerpt: "Enliten Lab -- Research"
sitemap: false
permalink: /research/
---

# Research

## DCNNN Toolbox for Contingency Screening with 100x Acceleration

_Summary provided by Yan Du_

Based on the latest developed deep convolutional neural network (deep CNN), we design a novel data-driven toolbox for power system security assessment, named as deep convolutional neural network for N-1 contingency screening, or DCNNN. The increasing penetration of renewable energy makes the traditional N-1 contingency screening highly challenging when a large number of uncertain scenarios need to be combined with contingency screening. The proposed DCNNN extracts the main features from power system raw data in a way similar to image processing, and it formulates a regression model for AC power flow calculation with high accuracy. Once the deep CNN is well-trained, it will obtain high generalization and can work in a nearly computation-free fashion for unseen instances such as topological changes in the N-1 cases and uncertain renewable scenarios, which is highly desirable for large-scale power system contingency screening.

The proposed DCNNN has been tested on several standard IEEE test systems and a large-scale European system, and it has also been compared with the model-based AC power flow calculation methods and traditional ANN to verify its accuracy. The data-driven DCNNN has been proved to be 100x times faster than the model-based method. The simulation results prove its potential for working as a fast power system contingency screening tool in real-time applications.

More details of this project can be referred to: [DCNNN]({{ site.url }}{{ site.baseurl }}/_pages/DCNNN.md) introduction. 
[DCNNN User Mannual]({{ site.url }}{{ site.baseurl }}/downloads/DCNNN_User_Manual.pdf)


## From AlphaGo to Power System Artificial Intelligence

_Summary provided by Yan Du_

Funded by the [NSF](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1809458), this project mainly focuses on utilizing the latest artificial intelligence (AI) techniques to solve the most complicated power system problems, like electricity market bidding and cascading outage screening. We are now living in an era that has witnessed the tremendous success of the deep learning (DL) technology in multiple fields like medical imaging, machine translation, and auto pilot, etc.  The DL method is like a black box. It “learns” the mapping between different variables via massive data mining and can automatically generate a proximate model representation without referring to analytical solution. Such data-driven method is especially desired when the problem is difficult to model due to hidden information or is computationally intractable due to high dimension or nonconvexity.

The application of deep learning in the power system is still at an initial stage. Like human board games, the power system engineers face quantities of practical grid planning and operation scenarios that are with extreme modelling complexity and computation overhead, where the data-driven deep learning method can serve as a highly reliable and efficient alternative way to overcome the above difficulties.  We have been working on implementing the deep convolutional neural network (deep CNN) for N-1 security assessment under uncertain operation scenarios, and the deep reinforcement learning (deep RL) for optimizing energy management for multi-microgrid and day-ahead market bidding strategy of GENCOs and have gained some promising results. We believe that there is high potential for the deep learning method to continue to outshine in future power system researches.

![]({{ site.url }}{{ site.baseurl }}/images/respic/DuAlphaGoPowerAi.png){: style="width: 600px; float: center; border: 10px"}



## A Distributed Energy Management Approach for Residential Demand Response

_Summary provided by Xiao Kou_

![]({{ site.url }}{{ site.baseurl }}/images/respic/KouDR.png){: style="width: 500px; float: right"}
Existing demand response (DR) research has primarily focused on the deployments for industrial customers. However, residential load accounts for 37% of the total electricity consumption in the United States (2013) and suggest a significant missed opportunity. Unlike industrial load, the residential load is composed of numerous low-power home appliances, and the electricity consumption habits of residential customers are highly varied and dynamic.


In this project, a distributed control scheme to coordinate large-scale residential demand response is proposed through coordination of Home Energy Management Systems (HEMS). In the proposed framework, end-use customers do not have to release the operating status of their home appliances to the load aggregator or their neighbors, which considerably protects the privacy and reduces the communication burden. Also, the distributed algorithm ensures the computational burden of the load aggregator and ensures the feasibility of the proposed algorithm for large-scale residential DR applications.


## Thermostatic load control for frequency regulation considering daily demand profile and progressive recovery

_Summary provided by Qingxin Shi_

![]({{ site.url }}{{ site.baseurl }}/images/respic/ShiThermostatLoad.png){: style="width: 350px; float: right; border: 10px"}
In recent years, the increasing penetration of renewable energy sources challenges power system frequency stability. Thermostatic loads can be controlled for frequency regulation with little impact on customers’ comfort. This research proposes a thermostatic load control (TLC) strategy, in which electric water heaters (EWHs) are utilized for primary frequency regulation (PFR) and heating, ventilation and air-conditioners (HVACs) are for secondary frequency regulation (SFR).


The innovation of this research includes two aspects. First, the demand profile modeling of the EWH and HVAC indicates that these two loads are complementary in the daytime. Therefore, they can provide a relatively stable frequency reserve. Second, the progressive load recovery is considered in the control scheme so that the load rebound effect can be avoided. With TLC strategy, the load aggregator can organize a large population of loads for the provision of a frequency reserve. Consequently, the requirement of generator spinning reserve is reduced.

## Graph Computing methods Applied in Large-scale Hybrid System Power System Analysis

_Summary provided by Wei Feng_

![]({{ site.url }}{{ site.baseurl }}/images/respic/FengGraph1.png){: style="width: 450px; float: center; border: 10px"}
![]({{ site.url }}{{ site.baseurl }}/images/respic/FengGraph2.png){: style="width: 450px; float: center; border: 10px"}

The rapid growing capacity of power transmission in modern power systems have led to an increase in building large-scale AC/DC hybrid system with high voltage direct current (HVDC) transmission lines. However, the added DC connections introduced great challenges into both physical world and power flow analysis, which is one of the most fundamental functions in energy management systems (EMS). To provide an efficient power flow analysis with better computing performance, the graph computing methods are employed in the sequential algorithm.

There are three main innovative aspects in this research. First, the power system is modeled as an intuitive graph with vertices and edges, and stored in graph database (GDB). Second, the graph partition is utilized to divide the whole network into several isolated AC grids by removing the DC connections. In this way, each independent subsystem can be solved at the same time with smaller sizes. Finally, for each fast decouple power flow (FDPF) in inner iterations and the data updating in outer iterations, the node-based parallel and hierarchical parallel computing is employed to speed up the computation. The proposed method is easy to be implemented in the existing software without compromising accuracy.

## Deep Learning Based Voltage Stability Assessment

_Summary provided by Mariana Magdy Mounir Kamel_

Voltage stability and voltage collapse have been a highly active research topic for decades. Even though voltage collapse has a low probability of occurrence, it certainly has a very high impact. Several major blackouts were reported to have been caused by voltage collapse.  In general, voltage instability problems would normally occur in heavily loaded systems where a small disturbance such as a line outage may result in a situation where the system is no longer able to meet its load power demand. Early detection of voltage instability is necessary to prevent the system from collapsing. Several voltage stability assessment techniques have been proposed in the literature in an attempt to assess proximity to voltage collapse.  However, a number of limitations have been reported in regards to those methods. One of the major issues which might render a given assessment method inapplicable is its computational complexity. This is true especially when the intention is to implement the assessment method in a real-time framework. As a matter of fact, till this day, devising a method which provides both fast and reliable assessment of system voltage stability remains to be a challenge.

This project aims at developing a deep learning based voltage stability assessment method which would be suitable for real-time implementation. Deep learning techniques, with their learning capabilities, offer high speed performance and therefore can be suitable for use in real-time applications. The proposed method would not only assess system stability and quantify its proximity to voltage collapse, but it should also optimize the decision on when, where, and which type of corrective measures to take in order to prevent the system from collapsing.

## Cyber-attack on electricity market operation

_Summary provided by Qiwei Zhang_

![]({{ site.url }}{{ site.baseurl }}/images/respic/ZhangCybersecurity.png){: style="width: 500px; float: center; border: 10px"}

We are studying how potentially profitable cyber-attacks will impact electricity market operations. The secure operation of today’s smart grids highly depends on the accuracy of measurements from state estimators. Independent system operators (ISOs) will retrieve these measurements to organize the electricity market. The strong coupling of power system cyber operations and physical operations will incite hackers to perform attack for monetary benefits.
