---
title: "Enliten Lab - Projects"
layout: textlay
excerpt: "Enliten Lab -- Projects"
sitemap: false
permalink: /projects/
---

# Projects
{:.no_toc}

## Table of Contents
{:.no_toc}

* TOC
{:toc}


## Another Market Simulator (AMS) 

_Summary provided by Qiwei Zhang_

The Another Market Simulator (AMS) is a power market simulation platform built within the CURENT large-scale testbed (LTB). AMS is the market module of LTB for solving steady-state market clearing and scheduling problems.  The current version of AMS is capable of solving three types of problems: (1) unit commitment (UC), (2) economic dispatch (ED), and (3) real-time ex-post pricing. The models in AMS are formulated and optimized with Gurobipy, and the simulation results can be outputted as a .xslx file or figure plot based on users’ preferences. The following figure shows a sample of UCED results plotted by AMS.

![]({{ site.url }}{{ site.baseurl }}/images/respic/AMS2.png){: style="height: 400px; float:right; border 10px;"}

The detailed instruction on AMS can be found in the user manual (click to download): [AMS User Manual]({{ site.url }}{{ site.baseurl }}/downloads/AMS_User_mannual_V0.pdf)

--------------

## Large Scale Testbed (LTB) for cyber-physical power grid simulation

![]({{ site.url }}{{ site.baseurl }}/images/respic/ltb-architecture-tall.gif){: style="height: 500px; float:right; border5 10px;"}

_Summary provided by Hantao Cui_ [![]({{ site.url }}{{ site.baseurl }}/images/more-info-button2.png){: style="width: 120px; float: center; border: 10px"}](LTB)

The CURENT Large Scale Testbed (LTB) for cyber-physical power grid simulation led by the CURENT research center (headquartered at The University of Tennessee) has been selected as a recipient of the 2020 R&D 100 Awards, which are known as the most prestigious innovation awards program for the past 56 years, honoring 100 great R&D revolutionary ideas and products each year in science and technology.

The CURENT LTB is a closed-loop software platform that continuously simulates the dynamics, communication, and control of modern power grids with high penetration of renewable energy. Below is a diagram of the LBT Main Architecture.
Since released in 2019, the LTB has received four licensed users (including two pending) and also played a critical role for research demonstrations to assist with 5 successes of funded proposals led by external users totaling $3.8 million in which the LTB lead Dr. Li serves as a collaborating site-PI or co-PI.

--------------

## Machine Learning Enabled Detection and Classification of Distribution Power System Outages

_Summary provided by Haoyuan Sun_

Distribution systems are geographically dispersed by nature. It may be affected by various factors, such as vegetation, weather, animal and human behaviors. Current response procedure to an outage massively rely on expert experience and tend to be time-consuming. Automatic outage event detection and classification will help to reduce the responding and restoration time. However, this issue is less addressed with existing research done in this focused area. In this applied research, a series of machine learning-based algorithms are proposed to detect and classify the outage events. Available data include three phase voltage & current waveforms and weather conditions during the forced distribution system outages. 

![]({{ site.url }}{{ site.baseurl }}/images/respic/Haoyuan_ORNL.png){: style="width: 800px; float: center; border: 10px"}

Our research initiates with a three-phase signal anomaly detection algorithm. The state of all the monitored signals can be reflected by a single signal. Once an anomaly is detected, the faulted phase could be identified by further processing the voltage and current waveform. Once this is completed, another algorithm is developed to classify the outages by their root causes, e.g., tree contact, animal contact, lightning, etc. Apart from weather condition and faulted phase information, we extract complex features that humans are unable to capture with machine learning methods from the voltage and current waveform and use them for the classification. An open source dataset from EPRI and also data from local utilities are used to test the proposed algorithms.


--------------


## Model Free Adaptive Control (MFAC) for Autonomous and Resilient Microgrids

_Summary provided by Buxin She_

Most existing inverter level controllers in microgrids, such as PI controller, sliding mode controller or H2 controller, are based on models. When applied to a new environment or the system has a large disturbance, parameters need re-tuning. The objective of this project is to develop a model-free adaptive control (MAFC) strategy for microgrids, so that the time consuming and inaccurate manual adjustment of microgrid controller parameters can be avoided. To address this concern, we plan to develop a reinforcement learning-based agent to tune the controller parameters adaptively. As shown in the left figure below, after offline training, the RL agent can dynamically adjust the PI controller gains (Kp and Ki) in the voltage recovery progress. In this way, the voltage of the common coupling point can adaptively track the predefined trajectory. The right figure shows that the control results are close to the desired value throughout the response time window. 

![]({{ site.url }}{{ site.baseurl }}/images/respic/Buxin_ESTCP.png){: style="width: 800px; float: middle; border: 10px"}

--------------



## Coordinated transactive control in a residential community

_Summary provided by Ian Schomer_

![]({{ site.url }}{{ site.baseurl }}/images/respic/Ian_ORNL.png){: style="width: 500px; float: right; border: 10px"}

Daily residential power consumption in aggregate tends to have a large peak that places stress on the distribution system and induces high operational costs. This work shows that coordinated transactive control of noncritical loads within a residential community or microgrid can help to alleviate peak-time stress on the distribution system by flattening the aggregate load curve. Treating the load forecaster as a high-fidelity, expensive black-box function, a new algorithm utilizing Bayesian optimization (BO) is proposed to achieve the best solution under uncertainty with minimal computing effort. The proposed BO algorithm manipulates the shape of the aggregate load by sending a unique transactive price signal to each home. The thermostatically controlled loads (TCLs) act out of self-interest in response to the given price while maintaining user comfort, and the Home Energy Management System (HEMS) exploits the thermal energy retention of the home for the benefit of the community.
The proposed algorithm was tested alongside a thermal home model designed with configurable comfort and energy usage parameters. Simulations on a multi-hour time horizon confirm consistent neighborhood-level peak power reduction, as well as energy cost savings for customers on average.


--------------

## Resilient Distribution Systems Enabled by Responsive Resident Building Loads

_Summary provided by Xiaofei Wang_

![]({{ site.url }}{{ site.baseurl }}/images/respic/Xiaofei_ORNL.png){: style="width: 500px; float: left; border: 10px"}

Inspired by the smart grid concept, the deployment of DERs including photovoltaic (PV), microturbine (MT), wind turbine (WT), and demand response (DR), have been increasing in the past decade in distribution systems. It is believed that DERs are driving the transition from a passive distribution system to a market-based one that aims to achieve the optimal allocation of all DERs.
In this project, a distribution level electricity market framework is established and a day ahead market clearing model is proposed. The distribution-level market aims to provide a platform for transparent energy transactions and economic allocations among various market participants. The distribution system operator (DSO) receives bids and offers from all market participants and makes financial settlements. Then, the DSO publishes distribution locational marginal price (DLMP) to all participants. Such price signals will guide the power generation/consumption of DERs. For example, residential users, via load aggregators (LAs), may optimize their load demands based on price signals to reduce their electricity bills. 


--------------

## [DCNNN Toolbox](DCNNN) for Contingency Screening with 100x Acceleration 


_Summary provided by Yan Du_ [![]({{ site.url }}{{ site.baseurl }}/images/more-info-button2.png){: style="width: 120px; float: center; border: 10px"}](DCNNN)

![]({{ site.url }}{{ site.baseurl }}/images/respic/DCNNN_toolbox.jpg){: style="width: 500px; float:right; border: 10px"}

Based on the latest developed deep convolutional neural network (deep CNN), we design a novel data-driven toolbox for power system security assessment, named as deep convolutional neural network for N-1 contingency screening, or DCNNN. The increasing penetration of renewable energy makes the traditional N-1 contingency screening highly challenging when a large number of uncertain scenarios need to be combined with contingency screening. The proposed DCNNN extracts the main features from power system raw data in a way similar to image processing, and it formulates a regression model for AC power flow calculation with high accuracy. Once the deep CNN is well-trained, it will obtain high generalization and can work in a nearly computation-free fashion for unseen instances such as topological changes in the N-1 cases and uncertain renewable scenarios, which is highly desirable for large-scale power system contingency screening.

The proposed DCNNN has been tested on several standard IEEE test systems and a large-scale European system, and it has also been compared with the model-based AC power flow calculation methods and traditional ANN to verify its accuracy. The data-driven DCNNN has been proved to be 100x times faster than the model-based method. The simulation results prove its potential for working as a fast power system contingency screening tool in real-time applications.


--------------

## From AlphaGo to Power System Artificial Intelligence

_Summary provided by Yan Du_

Funded by the [NSF](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1809458), this project mainly focuses on utilizing the latest artificial intelligence (AI) techniques to solve the most complicated power system problems, like electricity market bidding and cascading outage screening. We are now living in an era that has witnessed the tremendous success of the deep learning (DL) technology in multiple fields like medical imaging, machine translation, and auto pilot, etc.  The DL method is like a black box. It “learns” the mapping between different variables via massive data mining and can automatically generate a proximate model representation without referring to analytical solution. Such data-driven method is especially desired when the problem is difficult to model due to hidden information or is computationally intractable due to high dimension or nonconvexity.

The application of deep learning in the power system is still at an initial stage. Like human board games, the power system engineers face quantities of practical grid planning and operation scenarios that are with extreme modelling complexity and computation overhead, where the data-driven deep learning method can serve as a highly reliable and efficient alternative way to overcome the above difficulties.  We have been working on implementing the deep convolutional neural network (deep CNN) for N-1 security assessment under uncertain operation scenarios, and the deep reinforcement learning (deep RL) for optimizing energy management for multi-microgrid and day-ahead market bidding strategy of GENCOs and have gained some promising results. We believe that there is high potential for the deep learning method to continue to outshine in future power system researches.

![]({{ site.url }}{{ site.baseurl }}/images/respic/DuAlphaGoPowerAi.png){: style="width: 800px; float: center; border: 10px"}


--------------

## A Distributed Energy Management Approach for Residential Demand Response

_Summary provided by Xiao Kou_

![]({{ site.url }}{{ site.baseurl }}/images/respic/KouDR.png){: style="width: 500px; float: left"}
Existing demand response (DR) research has primarily focused on the deployments for industrial customers. However, residential load accounts for 37% of the total electricity consumption in the United States (2013) and suggest a significant missed opportunity. Unlike industrial load, the residential load is composed of numerous low-power home appliances, and the electricity consumption habits of residential customers are highly varied and dynamic.


In this project, a distributed control scheme to coordinate large-scale residential demand response is proposed through coordination of Home Energy Management Systems (HEMS). In the proposed framework, end-use customers do not have to release the operating status of their home appliances to the load aggregator or their neighbors, which considerably protects the privacy and reduces the communication burden. Also, the distributed algorithm ensures the computational burden of the load aggregator and ensures the feasibility of the proposed algorithm for large-scale residential DR applications.

--------------

## Thermostatic load control for frequency regulation considering daily demand profile and progressive recovery

_Summary provided by Qingxin Shi_

![]({{ site.url }}{{ site.baseurl }}/images/respic/ShiThermostatLoad.png){: style="width: 350px; float: right; border: 10px"}
In recent years, the increasing penetration of renewable energy sources challenges power system frequency stability. Thermostatic loads can be controlled for frequency regulation with little impact on customers’ comfort. This research proposes a thermostatic load control (TLC) strategy, in which electric water heaters (EWHs) are utilized for primary frequency regulation (PFR) and heating, ventilation and air-conditioners (HVACs) are for secondary frequency regulation (SFR).


The innovation of this research includes two aspects. First, the demand profile modeling of the EWH and HVAC indicates that these two loads are complementary in the daytime. Therefore, they can provide a relatively stable frequency reserve. Second, the progressive load recovery is considered in the control scheme so that the load rebound effect can be avoided. With TLC strategy, the load aggregator can organize a large population of loads for the provision of a frequency reserve. Consequently, the requirement of generator spinning reserve is reduced.

--------------

## Graph Computing methods Applied in Large-scale Hybrid System Power System Analysis

_Summary provided by Wei Feng_

![]({{ site.url }}{{ site.baseurl }}/images/respic/FengGraph1.png){: style="width: 450px; float: center; border: 10px"}
![]({{ site.url }}{{ site.baseurl }}/images/respic/FengGraph2.png){: style="width: 450px; float: center; border: 10px"}

The rapid growing capacity of power transmission in modern power systems have led to an increase in building large-scale AC/DC hybrid system with high voltage direct current (HVDC) transmission lines. However, the added DC connections introduced great challenges into both physical world and power flow analysis, which is one of the most fundamental functions in energy management systems (EMS). To provide an efficient power flow analysis with better computing performance, the graph computing methods are employed in the sequential algorithm.

There are three main innovative aspects in this research. First, the power system is modeled as an intuitive graph with vertices and edges, and stored in graph database (GDB). Second, the graph partition is utilized to divide the whole network into several isolated AC grids by removing the DC connections. In this way, each independent subsystem can be solved at the same time with smaller sizes. Finally, for each fast decouple power flow (FDPF) in inner iterations and the data updating in outer iterations, the node-based parallel and hierarchical parallel computing is employed to speed up the computation. The proposed method is easy to be implemented in the existing software without compromising accuracy.

--------------

## Deep Learning Based Voltage Stability Assessment

_Summary provided by Mariana Magdy Mounir Kamel_

Voltage stability and voltage collapse have been a highly active research topic for decades. Even though voltage collapse has a low probability of occurrence, it certainly has a very high impact. Several major blackouts were reported to have been caused by voltage collapse.  In general, voltage instability problems would normally occur in heavily loaded systems where a small disturbance such as a line outage may result in a situation where the system is no longer able to meet its load power demand. Early detection of voltage instability is necessary to prevent the system from collapsing. Several voltage stability assessment techniques have been proposed in the literature in an attempt to assess proximity to voltage collapse.  However, a number of limitations have been reported in regards to those methods. One of the major issues which might render a given assessment method inapplicable is its computational complexity. This is true especially when the intention is to implement the assessment method in a real-time framework. As a matter of fact, till this day, devising a method which provides both fast and reliable assessment of system voltage stability remains to be a challenge.

This project aims at developing a deep learning based voltage stability assessment method which would be suitable for real-time implementation. Deep learning techniques, with their learning capabilities, offer high speed performance and therefore can be suitable for use in real-time applications. The proposed method would not only assess system stability and quantify its proximity to voltage collapse, but it should also optimize the decision on when, where, and which type of corrective measures to take in order to prevent the system from collapsing.

--------------

## Cyber-attack on electricity market operation

_Summary provided by Qiwei Zhang_

![]({{ site.url }}{{ site.baseurl }}/images/respic/ZhangCybersecurity.png){: style="width: 400px; float: left; border: 10px"}

We are studying how potentially profitable cyber-attacks will impact electricity market operations. The secure operation of today’s smart grids highly depends on the accuracy of measurements from state estimators. Independent system operators (ISOs) will retrieve these measurements to organize the electricity market. The strong coupling of power system cyber operations and physical operations will incite hackers to perform attack for monetary benefits.
