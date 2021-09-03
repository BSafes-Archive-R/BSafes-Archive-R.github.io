---
layout: default
title: TECHNOLOGY CHALLENGES
parent: § Reshaping the Landscape of Future Manufacturing Software Defined Manufacturing  
grand_parent: R 
nav_order: 40 
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

## TECHNOLOGY CHALLENGES
While having the potential to revolutionize manufacturing and bring many advantages, there are several technical challenges that need to be addressed.

### Construction of Flexible and Universal Manufacturing Node
One of the most important key enablers for software defined manufacturing is the need for a flexible and universal manufacturing node, i.e., a node can produce a wide range of products and easily switch from one product to another. Without a large number of such nodes, SDL cannot have enough freedom to schedule production tasks to realize benefits such as innovation acceleration and better system efficiency.

One promising direction to implement such a flexible and universal manufacturing node is to utilize 3D printing and additive manufacturing technologies [12], [13]. Recent 3D printing and additive manufacturing technologies can use different materials to make many different products, from mechanical parts to medical tools and devices. Such production technologies can be easily integrated with SDL as they are fully controlled by software. Most existing 3D printing technologies are not scalable enough and too expensive for massive production. To overcome this challenge, it requires both advancement in material and print technology itself. Some works have been done along with these directions [14], [15].

Even if the universal manufacturing node is not mature at this time, the software defined manufacturing is still valuable: (i) The new framework can be applied to more specific sectors so the hardness of building a unified manufacturing node; (ii) Instead of using a single type of manufacturing nodes, the framework can support multiple types of manufacturing nodes. These strategies can help the early adoption of software defined manufacturing.

### Incentive Mechanism Design
To maximize the resource utilization, both the SDL and the PML infrastructures are shared by all practitioners. A natural question is: who will build and maintain these infrastructures? Building and running the SDL is relatively simple as it is very similar to the cloud/edge computing infrastructure we have today, and the major vendors (e.g., Amazon, Microsoft, and Google) have established a mature business model. The incentive mechanism that encourages the construction of manufacturing nodes in PML is less clear. To achieve some of the benefits of software defined manufacturing such as high supply chain resilience, it is better to deploy the manufacturing nodes globally, so practitioners have more choices when part of PML fails and disconnects from the system.

However, without a carefully designed incentive mechanism, investors may tend to build the manufacturing nodes into several clusters to reduce the cost of movement of components and attract more practitioners to schedule their jobs to manufacturing nodes that belong to a small number of clusters. This will form positive feedbacks and leads to a further concentration of manufacturing nodes, which is undesirable from the perspective of whole system resilience.

To avoid this from happening, the software defined manufacturing framework needs a compensation system to encourage deployment of manufacturing nodes in less favored locations, e.g., the system can collect a certain percentage of income from manufacturing nodes deployed in popular locations to balance the profits rate.

### System Security
The software defined manufacturing provides a disruptive way to organize manufacturing, maximizing the level of resource sharing to improve both flexibility and efficiency. To fully unleash the potential of this new way of organizing the manufacturing process, several security challenges need to be addressed:

*Isolation in the multi-owners/users infrastructure.* All components of SDL and PML are shared by multiple practitioners for efficiency and flexibility improvement. However, resource sharing also brings new challenges for the information managed and processed within the framework. Without a properly implemented isolation mechanism, a practitioner may leak valuable digital assets to an attacker. The isolation within PML is relatively easy to achieve as a manufacturing node will only carry out one task at a time. It is more complex to implement an isolation mechanism in the SDL. Existing technologies on virtual machines isolation [16] can be utilized to mitigate the challenge. But these methods usually rely on the assumption that the SDL infrastructure is trusted. When the SDL infrastructure is owned and managed by multiple parties, the situation is more complex and it is hard to make such an assumption.

*Trustworthiness of manufacturing nodes.* A manufacturing node accepts instructions from the SDL to finish the production process. The instructions usually include valuable intellectual property details (IPs) and leakage will lead to serious consequences. Another challenge is that the PML needs to guarantee received instructions are used in an expected way. For instance, a manufacturing node cannot “replay” received instructions to make extra products. One way to address these two challenges is to make sure that each manufacturing node in PML is trusted, i.e., it will always follow the protocol with computing nodes in SDL and keep information safe. To achieve this goal, trusted computing hardware can be integrated with each manufacturing node to offer a trusted execution environment (TEE) [17] for the control of the node. While this may not be able to guarantee that such nodes can be fully trusted, it can greatly reduce the attack surface.

*Coordination in a decentralized environment.* As SDL is owned and maintained by multiple parties, it is possible that two computing nodes that serve different practitioners want to send conflicting instructions to the same manufacturing node. In this case, the software defined manufacturing framework needs to provide a resolution mechanism. The emerging decentralized ledger (DL) technology provides a promising direction to address this issue. A DL is a data structure maintained by multiple peers, who run a consensus protocol to determine whether an instruction should be accepted, for example, blockchain technologies.

*Integration of DL and TEE for software defined manufacturing protection.*Integration of DL and TEE has the potential to address most of the security concerns in software defined manufacturing. Figure 3 provides an overview of the integrated security protection mechanism:

- Digital assets protection. The digital assets ownership information is managed by the DL in the same way as cryptocurrency, and the contents can be stored in the cloud in an encrypted format, which will only be decrypted when inside the TEE of a manufacturing node. 

- Instruction enforcement. The TEE integrated with the manufacturing node only accepts instructions through the DL, and the execution results are sent back to the DL for recording.

![Figure 3.](https://statics.bsafes.com/images/papers/Reshaping-the-Landscape-of-Future-Manufacturing-Software-Defined-Manufacturing-fig-3.png)
**Figure 3.** Security protection of the software defined manufacturing infrastructure.

### Scheduling Optimization
The modern supply chain has been studied a lot and many techniques have been developed to optimize its operation. The software defined manufacturing framework strives to achieve a balance between users’ flexibility and overall system performance. Optimization under this new framework is substantially different from existing problems. Specifically, the software defined manufacturing creates a dynamic environment, where the practitioners are able to interact with the whole manufacturing process through SDL and can thus bring a significant amount of uncertainties. For instance, a practitioner may cancel its production request through SDL to a production node (or a group of production nodes) in PML in the middle of the manufacturing process. This may either due to unexpected situations faced by the practitioner or the practitioner being malicious at the beginning.

Such “reoptimization-compatible” problem is a challenging topic in operations research as most of the common techniques in classical algorithmic design will fail. However, researchers have made some progress in the iterative augmentation method for integer linear programming [18], which is a fundamental mathematical tool for various optimization problems and can be utilized to partially address this specific scheduling optimization challenge.

### Compatibility
Most advanced manufacturing equipments use proprietary protocols and do not talk with each other. Under the software defined manufacturing framework, it is possible that the general manufacturing nodes are provided by different vendors that is not compatible with each other. To mitigate this challenge, a gateway can be deployed in the edge computing center which works as a proxy between practitioners and different manufacturing nodes. The practitioner can interact with the framework through a unified interface and does not need to worry about the specific equipment behind.

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
