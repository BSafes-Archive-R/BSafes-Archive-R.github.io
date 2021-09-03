---
layout: default
title: IMPACTS OF SOFTWARE DEFINED MANUFACTURING
parent: § Reshaping the Landscape of Future Manufacturing Software Defined Manufacturing   
grand_parent: R 
nav_order: 30 
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

## IMPACTS OF SOFTWARE DEFINED MANUFACTURING
By dividing the manufacturing ecosystem horizontally instead of vertically, the software defined manufacturing framework has the potential to transforms the business model of manufacturing as it breaks the silos and enables a free and fully competitive market. In this section, we summarize the potential impacts of software defined manufacturing when it becomes more mature and is widely adopted in practice.

### Accelerating Innovation
Innovation is playing a more important role in modern manufacturing. Within the current manufacturing ecosystem, the threshold to join the manufacturing business is becoming higher and higher, especially for advanced manufacturing that requires sophisticated and expensive equipment. Without access to these facilities, there is little a practitioner can do, e.g., conducting experiments to verify a new design or building a small number of products for the purpose of market feedbacks collection. Established big players will try to further enhance the barriers to maintain their monopoly position. Therefore, it prevents broad participation and indirectly hinders innovation.

The adoption of software defined manufacturing can fully change the game, and help to realize the concept given in social manufacturing [10], [11]. Under the new framework, the whole infrastructure (including both SDL and PML) does not belong to any specific practitioner and is accessible to the public. Similar to the scenario of cloud computing, one can utilize the resources by renting other than owning, and the cost is charged in the manner of pay-as-you-go. Therefore, one can easily test new ideas at a relatively low cost and increase the production scale easily when the concept is verified.

In summary, the new framework lowers the market access threshold and puts a new practitioner at the same starting point as his/her established competitors. Besides removing one of the most critical barriers for innovation in the manufacturing sector, it also encourages existing practitioners to invest more in R&D as traditional advantages of established players are greatly eliminated.

### Improving Supply Chain Resilience and Flexibility
Modern manufacturing usually involves a complex and long supply chain, where most practitioners focus on their own business and compromise a tiny part of the whole system. Under the current framework, this fine-grained division of work has been proved to be successful in maximizing production efficiency. But at the same time, the sophisticated supply chain also brings more uncertainties to the ecosystem. The effect of a failure of a single link in the system can cascade to other practitioners on the same supply chain, and disrupt normal operations. The recent COVID-19 pandemic has shown the fragility of such a complex supply chain. As some of the major economies are locked down, the original supply chains are disrupted and it is hard, if not impossible, to re-build a similar one in another place in a short time period.

With the software defined manufacturing framework, SDL can easily re-schedule information processing related works from failed/disconnected computing nodes to others without service disruption. PML consists of a large number of unified manufacturing nodes that are flexible to produce different things. Although these manufacturing nodes may have different outputs, they can largely replace each other. Even if a node with higher output fails, multiple production nodes with relatively lower outputs can be used to replace its role with limited impacts on the supply chain. The substitutability of production nodes in PML gives a practitioner more flexibility to schedule physical production tasks. At the early stage of software defined manufacturing, there can be several groups of production nodes with different functions. This adds another constrain but will not affect the structure of the new framework.

In practice, this process can even be fully automated by a re-schedule service hosted in SDL. The practitioner can provide certain constraints beforehand, and SDL monitors the current status of the whole system. When some of the resources involved in current production activity become unavailable, the service runs an algorithm to determine the possible re-scheduling options based on the constraints and availability information. The practitioner can either select one from the options or allow the re-schedule service to do it automatically.

### Facilitating and Enhancing Collaboration

The manufacturing sector can benefit significantly from collaboration due to the fine-grained division of works. However, collaboration under the existing paradigm is quite complex as each factory/entity is a closed system, and usually has limited and fixed partners. To initialize a new collaboration relationship, interested practitioners need to create a pair of dedicated interfaces between each other, which usually involves a lengthy administration process and cannot be reused with others.

Software defined manufacturing simplifies the process of collaboration from the following two perspectives: (i) Focusing on collaboration in SDL. As manufacturing nodes in PML are universal and completely controlled by computing nodes in SDL, two practitioners who want to collaborate only need to work in the cyber world to achieve consensus on the protocol for exchanging digital assets (e.g., designs, patents, and drawings) and provisioning adequate privileges to the other party to access their own resources in SDL. (ii) Open standards. The interfaces between major components of software defined manufacturing will be standardized, so the work that is done for one collaboration can be easily re-used for other collaborations. 

By utilizing the above two features, a market for collaboration can be built as part of SDL, where a practitioner can publish all types of demands to seek potential collaborators. Other practitioners who have a solution for the problem can then bid or negotiate on the platform to become a collaborator. This collaboration market is similar to a crowdsourcing platform that fosters collaborations, but is dedicated to the manufacturing sector and closely integrated with the software defined manufacturing framework.

### Improving Overall Efficiency
Ideally, a factory should maximize the utilization of its resources and meet all demands simultaneously. Under the current framework, this is very hard to achieve as a factory is built with fixed output capacity, but the demand keeps changing. When the output capacity and demand do not match, there is no way for a single factory to achieve the two goals at the same time. Even if the output capacity and demand match for a single factory, the actual output is also affected by upstream and downstream factories, which rely on the market mechanism to determine their outputs indirectly. Therefore, there are very likely mismatches of demand and supply, which causes underutilization and wastes resources.

There are two reasons for the above problem: lack of resource sharing and lack of information sharing. The software defined manufacturing solves this problem in a systematic way. Manufacturing nodes in PML are universal and shared by all practitioners, as long as practitioners have different peak demand times, SDL can easily do a load balancing to maximize the utilization of production nodes, which is similar to the scenario of cloud computing where physical servers are shared by multiple tenants with different peak demand times.

SDL also allows different practitioners to exchange demand/supply information easily and they can schedule production tasks only when there is a determined demand from others. Therefore, the demand and supply will be better matched and stocking cost will be reduced.

### Cost Reduction
The cost of manufacturing can vary significantly for different industries, and we only analyze the major factors in a qualitative manner to show the potential of cost reduction with software defined manufacturing.

The major factors of the cost of conducting business in manufacturing in a traditional way include: (i) Cost of infrastructure building (*B*); (ii) Cost of producing (*P*), including material and labor cost; and (iii) Cost of the supply chain (*S*). While *P* and *S* are proportional to the output *O, B* is relatively independent of *O*. Therefore, the cost of each unit is *P/O* + *S/O* + *B/O*. Under the new framework, a practitioner does not need to invest in his/her own infrastructure but pays to rent necessary resources to create the manufacturing system when needed, which is denoted as *R*. The practitioner still needs to cover the costs of producing (*P'* ) and supply chain (*S'* ). But in this case, *R* is also proportional to *O*. In other words, *R/O* is roughly a constant value under software defined manufacturing framework. For the same output *O*, the cost of each unit is *P'/O* + *S'/O* + *R/O*.

The cost of producing is similar for both cases (i.e.,* P = P'* ), and the supply chain cost for software defined manufacturing can be cheaper as the practitioner has more flexibility in the optimization of the supply chain (i.e., *S > S'* ). The relationship between *B* and *T* is more complicated. When the infrastructure is fully utilized (*O* is maximized), *B/O < R/O*. However, when *O* is smaller, we have *B/O* > *R/O*. In summary, when O does not reach the full capacity of the manufacturing infrastructure, *P/O* + *S/O* + *B/O* >*P'/O* + *S'/O* + *R/O.*

From the infrastructure owner’s perspective, although he/she can only collect a rent fee that is proportional to the output, the facility can be rented to multiple practitioners.

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
