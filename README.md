# MECSim

MECSim: A Comprehensive Simulation Platform for Multi-Access Edge Computing

# Please cite it as (Kindly do not use the github link):

Akhirul Islam and Manojit Ghose (2026). MECSim: A Comprehensive Simulation Platform for Multi-Access Edge Computing

Bibtex:
```groovy
@article{ISLAM2026103706,
title = {MECSim: A comprehensive simulation platform for multi-access edge computing},
journal = {Journal of Systems Architecture},
volume = {173},
pages = {103706},
year = {2026},
issn = {1383-7621},
doi = {https://doi.org/10.1016/j.sysarc.2026.103706},
url = {https://www.sciencedirect.com/science/article/pii/S138376212600024X},
author = {Akhirul Islam and Manojit Ghose},
keywords = {Simulation, Multi-access edge computing, Modeling, DVFS-enabled devices, Edge simulator, MEC simulator, Task offloading},
abstract = {The rapid growth of CPU-intensive and latency-sensitive applications has intensified the need for efficient resource management within edge computing environments. While existing simulators such as iFogSim, EdgeCloudSim, and PureEdgeSim have contributed significantly to edge computing research, they lack comprehensive support for modeling modern hardware heterogeneity, energy-aware mechanisms, service providers’ economic models, dependent task modeling, and reliability-driven task management. This paper presents MECSim (multi-access edge computing simulator), an enhanced simulation framework that extends PureEdgeSim to enable realistic modeling of heterogeneous, cooperative, and fault-tolerant edge computing ecosystems. MECSim supports multi-data-center clusters along with dynamic voltage and frequency scaling (DVFS) capable user devices for energy-efficient operation. The framework further integrates dependent-task modeling, cost and profit evaluation for service providers, and reliability mechanisms via transient-failure simulation, caching, and task replication. We have implemented five state-of-the-art approaches, demonstrating the effectiveness of our simulation platform and building confidence in its practical utility to handle diverse system architectures. With its extensible architecture and comprehensive modeling capabilities, MECSim provides a promising platform for future research on energy-efficient, profit-driven, and fault-tolerant task offloading and scheduling in heterogeneous MEC environments. The results also demonstrate that MECSim achieves a 44.13% (on average) reduction in simulation time compared to EdgeCloudSim. In addition, we have conducted experiments using dispersion-aware metrics to quantify variability and stability across 50 independent runs, thereby enabling a more robust and reliable performance evaluation.}
}
```

## 📖 Overview
MECSim (multi-access edge computing simulator), an enhanced simulation framework that extends PureEdgeSim
to enable realistic modeling of heterogeneous, cooperative, and fault-tolerant edge computing ecosystems.
MECSim supports multi–data-center clusters along with dynamic voltage and frequency scaling (DVFS) capable 
user devices for energy-efficient operation. The framework further integrates dependent task modeling, cost 
and profit evaluation for service providers, and reliability mechanisms through transient failure simulation, 
caching, and task replication.


MECSim offers many features as PureEdgeSim: 

1. Realistic modeling of edge computing scenarios (and its related computing paradigms).

*   It supports devices heterogeneity (sensors, mobile devices, battery-powered..).
*   It supports the heterogeneity of their means of communication (WiFi, 5G, 4G, Ethernet..).
*   Realistic modeling of computing infrastructure (modeling computational tasks, infrastructure topology...).
*   Realistic network model (Latency, bandwidth allocation, support for peer to peer communications, routing..).
*   Realistic mobility model.
*   Realistic energy model.

2.    The support for online decision making (tasks orchestration, scheduling, etc.).

3.    The study of QoS-aware architectures and topologies.

4.    Efficiency and Scalability.

*   MECSim supports the simulation of thousands of devices.
*   MECSim supports scenarios with longer simualtion time (even +24 hours).

5.    A wide collection of metrics.

*   Delays: execution time, waiting time, network time.
*   CPU utilization.
*   Network utilization: Average bandwidth, total traffic...
*   Energy consumption: The energy consumption of computing nodes (Cloud, edge/fog servers,edge devices), the remaining energy of battery-powered devices, the energy consumption of WAN, MAN, and LAN networks, and the enrgy consumption of WiFi, Cellular (5G, 4G,..) and Ethernet.
*   Task success rate and reason of failure (the rate of tasks failed due to the lack of resources, due to mobility, due to latency, or due to the death of edge devices when they run out of battery).
*   and many others.

7.    Extensibility: Users can implement their scenarios and integrate their models without modeifying PureEdgeSim codebase.
8.    Wide Applicability

*   Mist computing scenarios, mobile ad hoc edge computing, fog computing,...
*   Worklaod orchestration, scheduling, caching...

9.    Ease of use.

10.    Reliability.

11.    Correctness.

## 🧰 Exclusive Features

MECSim supports following exclusive features.
1. It supports multi-DC cooperative edge cluster with heterogeneous edge servers in terms of
   computing and storage capacities. 
* It also supports modern hardware supports in terms of computing and storage (GPU, PiM, SSD).
* It enhanced the task latency calculation to make it more reliable by addimg factors like IO time,
  data transfer between memory and processor time in addition to CPU time. Existing work only considers the CPU time.
* It supports task execution result caching using Broker

2. It supports dynamic voltage and frequency scaling (DVFS) devices and it helps in reducing energy consumption.

3. It supports dependent task modeling based on directed acyclic graphs (DAGs).
* It has  the capability to identify task criticality
* It can calculate reliability of a task and based on it can find low reliable tasks
* It supports reliability-aware offloading and selective task replication.
* It has option to simulate user device failure
 

## 👩🏽‍💻 How to Use

There are several ways to use PureEdgeSim; however, it is strongly advisable to run MECSim via a Java development environment, like Eclipse or IntelliJ IDE. A set of predefined examples is provided under the “/examples“ directory, which should allow anyone to become familiar with MECSim.
