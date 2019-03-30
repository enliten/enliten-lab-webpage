---
title: "Enliten Lab - Research"
layout: textlay
excerpt: "Enliten Lab -- Research"
sitemap: false
permalink: /research/
---

# Research

## From AlphaGo to Power System Artificial Intelligence

_Summary provided by Yan Du_

Funded by the [NSF](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1809458), This project mainly focuses on utilizing the latest artificial intelligence (AI) techniques to solve the most complicated power system problems, like electricity market bidding and cascading outage screening. We are now living in an era that has witnessed the tremendous success of the deep learning (DL) technology in multiple fields like medical imaging, machine translation, and auto pilot, etc.  The DL method is like a black box. It “learns” the mapping between different variables via massive data mining and can automatically generate a proximate model representation without referring to analytical solution. Such data-driven method is especially desired when the problem is difficult to model due to hidden information or is computationally intractable due to high dimension or nonconvexity. 

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

