---
layout: default
title: OVERVIEW OF THE SOFTWARE DEFINED MANUFACTURING
parent: § Reshaping the Landscape of Future Manufacturing Software Defined Manufacturing   
grand_parent: R 
nav_order: 20 
---
<style>
.dont-break-out {
  /* These are technically the same, but use both */
  overflow-wrap: break-word;
  word-wrap: break-word;

     -ms-word-break: break-all;
  /* This is the dangerous one in WebKit, as it breaks things wherever */
  word-break: break-all;
  /* Instead use this non-standard one: */
  word-break: break-word;
}

.youtube-container {
    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 56.25%;
}
.youtube-video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

</style>

<div class="dont-break-out" markdown="1">

1. TOC
{:toc}

## OVERVIEW OF THE SOFTWARE DEFINED MANUFACTURING
Software defined manufacturing breaks the boundaries between different factories by extending existing ideas such as cloud based manufacturing and 5G, and brings resource sharing and collaboration to a new level, which are critical for future manufacturing.

### Architecture of Software Defined Manufacturing
Figure 1 presents the major differences between the current practice of utilizing information technology to modernize manufacturing infrastructure and the future software defined manufacturing infrastructure. As depicted on the left side of Figure 1, current R&D efforts such as Industry 4.0 [1], [8] focus on modernization and digitization of each single manufacturing factory by introducing automated tools like robots and AI components to reduce the working intensity, improve production efficiency, and eliminate potential failures with better prediction. Under this framework, the potential of each factory can be maximized and the productivity of the whole sector scales vertically.

On the right side of Figure 1, instead of splitting the manufacturing sector vertically into silos, software defined manufacturing framework breaks the boundaries and makes it an open, sharable ecosystem. Specifically, software defined manufacturing divides the industry ecosystem horizontally into two layers, the physical manufacturing layer and the software definition layer, which are accessible to and shared by all practitioners.

- *Physical manufacturing layer (PML)*. The framework requires the physical manufacturing layer to support universal production and be as flexible as possible. The PML is composed of a group of sites, and each site has a set of equipment that can be controlled by software for manufacturing. Here the equipment can be a 3D printer or other instruments that have the capability to make a wide range of different items. The PML is shared by multiple practitioners. Although it is a challenge that each site can support all manufacturing activities, it is feasible to build such sites for a specific sector to cover the majority of the production activities. The auto industry has adopted a similar strategy by introducing car platforms to increase the percentage of sharable components [9]. The industry has been pursuing *flexible manufacturing* for a long time, which aims at the ability to deal with mixed parts, allow variation in parts assembly, and support production volume and design changes. Most of these features are aligned with the goals of PML. Leading equipment manufacturers like ABB and Leidos have developed a variety of technologies to support flexible manufacturing that can be leveraged for the construction of PML. At the early stage of software defined manufacturing, PML can also include more than one type of site to support multiple sectors. But the sharing nature of these sites does not change.

- *Software definition layer (SDL).* The SDL is responsible for everything except the actual manufacturing, including design, development, simulation, and control of the whole information infrastructure of the manufacturing process (e.g., sending instructions and receiving feedback from PML sites and equipment). SDL can be further decomposed into two sub-layers, the computation layer and the communication layer. The computation layer manages a variety of valuable digital assets for a practitioner such as designs and technological processes, which determine a practitioner’s capability and level of efficiency to make products. The communication layer is a bridge that connects the cyber world and the physical world, which supports reliable connections between the computation infrastructure and the physical manufacturing infrastructure. The communication layer is also configurable and controllable through the computation layer, i.e., a practitioner can decide the features of connections needed for the manufacturing tasks, such as bandwidth and latency. Similar to PML, the SDL infrastructure is shared by multiple practitioners. The difference is that SDL is shared across different sectors. At the same time, a practitioner can store and manage private assets using SDL for their own usage, trading with others, or collaboration with other practitioners.

### Components and Usage of Software Defined Manufacturing

There are three types of components in the software defined manufacturing infrastructure. 

- Computing node. A large number of computing nodes compromise the computation layer of SDL, which is responsible for computation and storage tasks. There are different ways to organize computing nodes, and a simple way is to have a centralized party to provide and manage all computing nodes, like the current practice in cloud computing. 

- Communication channel. Communication channels are also part of SDL and are responsible for providing reliable connections between other nodes in the system. As 5G infrastructure is deployed, the computing nodes and communication channel can converge and be managed by a single operator. 

- Manufacturing node. These nodes compromise the PML. A manufacturing node is highly autonomous and can be owned by anyone. After it connects to the framework, it is fully controlled by the SDL for daily operations. 

A practitioner *p* interacts with the software defined manufacturing as follows: 

- *p* logs into its management portal hosted in the cloud, which is part of the software defined manufacturing framework. Through the management portal, p can see the demand and supply information, all its digital assets, the current status of manufacturing nodes, and other services (e.g., scheduling tool) it subscribed to. 

- *p* finalizes the production plan and submits instructions to manufacturing nodes through the software defined manufacturing framework. 

- A manufacturing node carries out the production according to received instructions (e.g., technological process and quantity).

A financial settlement protocol is integrated with the above process, and the payment option can be part of the manufacturing node status.

Figure 2 shows a concrete example of software defined manufacturing architecture from a practitioner’s perspective. SDL is built and implemented using the cloud-edge computation infrastructure, which includes a limited number of cloud computing data centers with plenty of computation and storage resources and a large number of edge computing data centers that are physically distributed. The cloud (the centralized computing infrastructure in Figure 2) is responsible for interacting with the practitioner and most of the computation and storage intensive manufacturing activities related R&D work. As the physical manufacturing facilities (manufacturing node) are geographically distributed, multiple edge data centers (the distributed computing infrastructure in Figure 2) are utilized to control the operations of manufacturing nodes that are close to them. The communication infrastructure is integrated as part of the cloud-edge computation system.

A practitioner utilizes a cloud data center to finish the R&D work of a new product. The cloud also maintains the current statuses of all manufacturing nodes that are essential for scheduling, including locations, production capacities, planned workloads, and transportation information. When there are multiple types of manufacturing nodes in the system, the type information is also provided. The practitioner utilizes the information to schedule the physical production works. If the product is a sub-component of another product, the practitioner also takes the schedules of collaborators into consideration when determining their own plan.

After the schedule is finalized, instructions are distributed to edge data centers, and the edge data centers will coordinate with manufacturing nodes to start the production process. Even for a single practitioner, the manufacturing process can involve multiple steps. In this case, it is possible several manufacturing nodes are utilized. The end product of one manufacturing node is the raw product of another manufacturing node, and transportation is involved as part of the schedule.

![Figure 2.](https://statics.bsafes.com/images/papers/Reshaping-the-Landscape-of-Future-Manufacturing-Software-Defined-Manufacturing-fig-2.png)
**Figure 2.** A use case of the software defined manu- facturing from a practitioner’s perspective.

Under the software defined manufacturing framework, SDL and PML do not belong to any specific entity. Both SDL and PML are provided virtually to all practitioners, and the resource allocation process is transparent to them. In other words, each practitioner believes is the only one using the system and does not need to be aware of other practitioners in the system. In Figure 2, resources covered by the shaded area are allocated to the practitioner, and from the view of the practitioner, all these resources are used exclusively. But in reality, these resources can also be utilized by another practitioner.

***

#### Table of Contents
{: .no_toc}

<ul><li> <a href="/docs/R/Reshaping-the-Landscape-of-Future-Manufacturing-Software-Defined-Manufacturing-1/">
INTRODUCTION</a></li><li> <a href="/docs/R/Reshaping-the-Landscape-of-Future-Manufacturing-Software-Defined-Manufacturing-2/">
OVERVIEW OF THE SOFTWARE DEFINED MANUFACTURING</a></li><li> <a href="/docs/R/Reshaping-the-Landscape-of-Future-Manufacturing-Software-Defined-Manufacturing-3/">
IMPACTS OF SOFTWARE DEFINED MANUFACTURING</a></li><li> <a href="/docs/R/Reshaping-the-Landscape-of-Future-Manufacturing-Software-Defined-Manufacturing-4/">
TECHNOLOGY CHALLENGES</a></li><li> <a href="/docs/R/Reshaping-the-Landscape-of-Future-Manufacturing-Software-Defined-Manufacturing-5/">
CONCLUSION</a></li><li> <a href="/docs/R/Reshaping-the-Landscape-of-Future-Manufacturing-Software-Defined-Manufacturing-6/">
REFERENCES</a></li></ul>

***

</div>
