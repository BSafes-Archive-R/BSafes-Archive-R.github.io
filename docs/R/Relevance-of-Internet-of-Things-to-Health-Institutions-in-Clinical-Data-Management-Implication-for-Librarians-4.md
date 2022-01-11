---
layout: default
title: DEFINING THE PROCESS FLOW
parent: § Relevance of Internet of Things to Health Institutions in Clinical Data Management - Implication for Librarians  
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

## DEFINING THE PROCESS FLOW
A summary of key data management tasks is presented below and will be used as a focus for performance measurement:

- *Data collection*: Data can arrive in an electronic format, such as laboratory data from central laboratories, diary card data collected on hand-held computers or via interactive voice response systems, or more directly via remote data entry systems and remote data capture solutions.

- *Pre-entry data review* (secondary monitoring). Often, a pre-entry manual review of all source CRF data is made to ensure completeness of data. Some data may be coded at this stage to support the data entry process. Data queries may also be raised at this stage.

- *Data entry*. Following receipt of data from the investigator site, data are keyed or loaded onto the clinical database. Most data entry teams enter CRF data via an independent double data entry process with either a file extract and compare process or via an on-line verification process to ensure data quality at this key stage in the development of the database

- *Data validation*. Data are cleaned in a batch process using validation programmes which have been specified and developed before data entry commences. The majority of data queries are generated at this stage

- *Term coding*. Adverse event data, concurrent medications and medical conditions are often coded using standard dictionaries both using an auto encoder and via manual coding. Again, this is often a batch process.

- *Database editing*. The developing database is edited following batch receipt of resolved data queries from the field.

Process tasks listed above are by no means comprehensive but typically summarize the inprocess flow for data management

### The Proposed Information System Architecture Based on IOT Technologies
As confirmed by a survey in several Swiss hospitals at 2009 (Rondel, Varley & Webb, 2020), 64% of them replied that the healthcare sector is a complex and heterogeneous economic sector and cannot be compared to other industry sectors where Control Objectives for Information and related Technology (CobiT) and other IT governance framework have been successfully applied; hence, the use of this particular information structure. Here, specific sensors are used to collect comprehensive physiological information and uses gateways to send data to the server on the Cloud for analysing and storage. Information is sent after to medical-staff wirelessly. Our proposition is shown in the figure below


Fig 2 A Proposed Structure
![Fig 2 A Proposed Structure](https://statics.bsafes.com/images/papers/Relevance-of-Internet-of-Things-to-Health-Institutions-in-Clinical-Data-Management-Implication-for-Librarians-fig-2.png)


For data collection the use of the IoT solutions greatly improves the quality of care through continuous attention and lowers the cost of care by eliminating the need for a medical-staff to actively engage in data collection. In addition, the technology can be used for remote monitoring using small, wireless solutions connected to patients through the IoT capabilities. Data is collected from different sources: Wearable devices or from sensors (installed on different equipment).

- The Middleware plays the role of a gateway, it intercepts data sent by the various sensors to the software platform located in the cloud to be stored and analysed. The middleware performs an authentication operation to identify the device; it formats data under to specific shape before sending it to the server. The formatting operation facilitates the server work, it minimises the time of data recognition operation.

- The IoT Platform Components: In what follows the most important constituents of the server on the Cloud architecture are highlighted. First, the register contains a list of IoT devices and different equipment that collect data, it used to control and to avoid any external and unwanted attempts to connect to the server or to the gateway.

- The Device Management module: is used to manage objects connects to the IoT platform. User can add, remove and configure devices remotely.

- Collaborative planning module: this module allows an efficient planning with a collaborative manner. Hence health care task planning process is fundamentally a collaborative task that requires the participation of many health care experts with different skills working simultaneously on same cases. It’s based on a collaborative planning approach and it constitutes an evolution of planning environments toward new shared workspaces supporting collaboration.

- The Data Storage module takes care of the collected data storage either inside or outside the hospital. It uses relational databases as well as big data techniques or any data storage technology. This section provides the user a fast, secure and efficient access to all patient, medical and other resources information.

- The tGRC module enables the health institution to manage risk and regulatory issues across the organization. It provides a set of essential services and functional components that encompass various areas of risk and compliance management.

- The tGRC solution legal register offers access to the legal universe for each act. Fully searchable, tGRC solution gives the needed law easily and rapidly. The stakeholders can give feedback on the published information. This feedback is sent to the rules database. Finally, the rules administrator can improve and communicate about this information.

Accordingly, the proposed modelling step aims at a balanced consideration of both compliance and risk factors while incorporating the risk attitude of governance maker regarding the IoT systems specificity and the Cloud offers.

The model aims to set goals to reach global objectives. Formally objectives are:
![](https://statics.bsafes.com/images/papers/Relevance-of-Internet-of-Things-to-Health-Institutions-in-Clinical-Data-Management-Implication-for-Librarians-fig-3.png)

These three objectives for IoT systems based on tGRC concepts form a solid basis for evaluating the IoT systems and Cloud offers solution which could be extended in practice by more detailed and specific objectives. For example, the security objectives have to be detailed by authentication, authorization, accounting, etc. The model developed here is meant to act as a risk minimization and compliance maximization tool, that is, it is supposed to identify the Cloud Computing service or the combination of services which causes the optimal cost for an organization by taking risk and compliance issues into account.

Reasons or objectives of introducing IOT in clinical data management cannot be over emphasized which include: to obtain valid patient data via Case Record Forms (CRFs) as required by the protocol; ensure immediate availability of data in the company (the time gap from site to database should be minimal); ensure immediate processing of incoming data (including plausibility/validity checking/database finalization); provide validated databases, both the initial application and upgrades, for product registration and other company needs; enable compilation of global and project databases composed from local databases (international clinical trial) for statistical reporting and tabulations; provide necessary access to the data of an ongoing trial to satisfy drug safety aspects, ethical and legal requirements; fulfill GCP requirements with respect to clinical data processing. Just as the objectives are all encompassing, so also are the objectives and these makes IOT a necessity in health institutions.

### Importance of IOT in health management
From all indications, it will not be out of place to state here that the importance of IoT is to connect smart objects (referring to things) to the Internet in a transparent way thereby leading to an exchange of data between all things, and bring health users information in a more secure way. According to Riazul, Daehan, and kwak, cited in Gonçalo and Vitor (2019) healthcare is one of the most attractive applications fields for IoT making available the possibility of many medical applications such as remote health monitoring, fitness programs, chronic diseases, and elderly care. As we all know, healthcare is an important priority for all (governments inclusive) as it relates to population growth, rural urbanization, declining birthrate, population aging, economic growth and social unbalanced resource utilization. Some social problems have become increasingly apparent in the healthcare field; some of these issues in healthcare that IoT can combat in a most effective way (Gonçalo & Vitor, 2019) includes:

- health management level and the incapability of responding to emergency;

- serious shortage in medical staffs and institutional facilities especially in rural areas, lack of medical facilities, low level of treatment, inadequate healthcare system;

- Imperfect diseases prevention system cannot meet the national strategy requirements to safeguard the health of the citizen resulting in an heavy burden on economy, individuals, families and State;

- Inadequate disease prevention and early detection capability

- There are technologies that are useful in healthcare environment which can be adopted in IOT-based healthcare system to the benefit of both patients and provider stand to benefit from.

- Reduction in cycle time from protocol development to report

- Improved Regulatory Compliance (complete audit trails, CANDAs) 

- Improved data integrity and quality, tracking techniques 

- Improved efficiency and utilization of resources

- Facilitated clinical research monitoring capabilities 

- Improved project management and planning capabilities 

- Reduction or maintenance of project costs.

### Challenges associated with the use of IOT such as cyber security, lack of basic infrastructure
One of the major challenges in Nigeria over the years is the issue of security which networks is not excluded. Therefore, security, privacy and trust are critical factors for IoT applications as well. Laith et al. (2018) were of the opinion that when packets are routed through different links and devices to reach ultimate receiver on the internet, measures should be taken so that the confidentiality and integrity of the data is maintained. It was clearly stated that:

> IoT devices are low power constrained devices, therefore, already established cryptographic solutions cannot be directly applied in the IoT scene. More so, the integration of application in the network infrastructure is focused on only achieving the functionality rather than holistically considering the security requirements when the application is designed (Laith et al. 2018, p.5).

There were warning from cybersecurity experts on IoT as the most vulnerable technology as they expect more targeted attacks on existing and emerging infrastructures such as data theft, physical injury, ransomware for smart homes or smart cars among others. Other challenges include:

Trust and data integrity which enables one to ensure the data sent has not changed from the moment it is sensed until it reaches the final destination. This involves verifying the data and validating the verification certificate. Trillion points of vulnerability is a situation where each device connected to IoT represents a potential risk and leads to questions - how confident can an organization be of the data gathered and the integrity of the data sent? How to make sure data has not been interfered or compromised with? These and many more were the issues arising from IOT vulnerability.

Data protection: considering a country like ours where copyright protection has not been properly implemented in an online environment one begins to be more curious if there will be require law to be designed to protect and control individual and organization data gathered by sensors or applications and stored to be part of a filing system.

Data privacy: is to protect the data from exposure in the IoT environment. For instance, any logical or physical entity can be given a unique address and the ability to communicate automatically over the network.

### Challenges associated with the use of IoT
As mentioned earlier, one major challenge in Nigeria over the years is the issue of security which networks is not excluded. Therefore, security, privacy and trust are critical factors for IoT applications as well. IoT devices are low power constrained devices; therefore, already established cryptographic solutions cannot be directly applied in the IoT scene. There were warning from cybersecurity experts on IoT as the most vulnerable technology as they expect more targeted attacks on existing and emerging infrastructures such as data theft, physical injury, ransom-ware for smart homes or smart cars among others. Data Privacy is to protect data from exposure in the IoT environment. For instance, any logical or physical entity can be given a unique address and the ability to communicate automatically over the network.

***

#### Table of Contents
{: .no_toc}

<ul><li> <a href="/docs/R/Relevance-of-Internet-of-Things-to-Health-Institutions-in-Clinical-Data-Management-Implication-for-Librarians-1/">
INTRODUCTION</a></li><li> <a href="/docs/R/Relevance-of-Internet-of-Things-to-Health-Institutions-in-Clinical-Data-Management-Implication-for-Librarians-2/">
Literature Review</a></li><li> <a href="/docs/R/Relevance-of-Internet-of-Things-to-Health-Institutions-in-Clinical-Data-Management-Implication-for-Librarians-3/">
DOMAIN MODEL FOR HEALTH INSTITUTION APPLICATION BASED ON IOT</a></li><li> <a href="/docs/R/Relevance-of-Internet-of-Things-to-Health-Institutions-in-Clinical-Data-Management-Implication-for-Librarians-4/">
DEFINING THE PROCESS FLOW</a></li><li> <a href="/docs/R/Relevance-of-Internet-of-Things-to-Health-Institutions-in-Clinical-Data-Management-Implication-for-Librarians-5/">
CONCLUSION</a></li><li> <a href="/docs/R/Relevance-of-Internet-of-Things-to-Health-Institutions-in-Clinical-Data-Management-Implication-for-Librarians-6/">
REFERENCES</a></li></ul>
***

</div>
