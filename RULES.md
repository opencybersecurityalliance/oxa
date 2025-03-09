# Rule of engagement 

 

## Preamble 

The Open XDR Architecture (OXA) project aims to create an open and collaborative architecture for eXtended Detection and Response (XDR). OXA aims to offer a framework that brings together complementary solutions and players by aggregating the different capabilities within an ecosystem to offer composable security that meets the needs of organizations.  

This Rules of Engagement (ROE) establishes the conditions of membership, the terms of participation, and the resulting benefits for OXA members. 

 

## 1. Conditions to join the OXA project 

### 1.1 Eligibility criteria 

To become a member of the OXA project, an organization must be an entity or a company working in the field of IT security and offering a solution or tool that can be integrated in an Open XDR approach.  

### 1.2 Acceptance of the OXA Principles 

Each member must agree to OXA's core principles, such as interoperability, modularity, and sharing. The compliance with security norms and standards that can leverage these principles are preferred.  

### 1.3 Open-Source Commitment 

OXA members are expected to share open-source principles, stating that individual contributions that benefits to the community should be reversed to the project. It enables open, transparent and collaborative milestones to achieve better and faster project achievements. 

 

## 2. Involvement process 

### 2.1 Application and membership 

Any organisation interested in OXA can join the initiative without any special application process.  Membership is gained when the organization starts to participate to the project. 

### 2.2 Participation  

Different kind of contributions can be made as detailed in the CONTRIBUTING file. 

### 2.3 Active Engagement 

OXA members are expected to actively participate in discussions, development work, and community activities. Active engagement is essential to ensure the success and sustainability of the project. 

### 2.4 Public communication 

Any organization being part of discussions, mailing list or contributing to the repository can claim to be a member OXA and use this membership at their will. 

Labels will be the formal way to showcase the membership based on a public reference. 

The OXA project asks its members to communicate positively about the project and to always use respectful wording regarding the project, its governance and its members.  

## 3. Conditions for benefiting from OXA 

### 3.1 Access to Resources 

OXA members will have privileged access to project upcoming milestones, including technical documents, code updates, and community discussions. 

Any visitor can also use the public repository of OXA to leverage it on his side as long as it is aligned with the LICENCE file content. 

### 3.2 License and Use 

Solutions developed within the framework of OXA are made available under open source license. Members may use, modify, and distribute these solutions in accordance with the terms of the license defined in the LICENCE file. 

### 3.3 Label and Use 

As described in the LABEL file, organization willing can pretend to an OXA label, describing how they leverage the framework. Depending on the level, the validation is self-declarative for the first levels and is reviewed for the upper levels. 

Once an organization becomes label grantee, it can exploit the label logo widely and for free. 

## 4. Collaboration between Products  

### 4.1 Interoperability 

OXA members undertake to design their internal technological architecture taking into account interoperability with the other components of the project. The use of open standards and norms is the preferred condition for good interoperability. OXA aims to densify the potential interactions between cybersecurity product that can play an active role in Security Operations. 

### 4.2 Standards used in OXA 

Open standards will have to be leveraged to allow maximum interoperability in data structuring, orchestration, automation, intelligence sharing and connection via an API.  

#### 4.2.1 Data ingestion  

The notion of data ingestion refers to the process of collecting data from different sources and speaking different languages to structure it in a coherent way and translate it in such a way that it can be analyzed and used. 

In concrete terms, it involves gathering information from various security sensors that do not necessarily communicate with each other and centralizing it in a unified system. 

To do this, OXA will rely on a transformation step and will exploit best practices in terms of formats used for ingestion. To date, three different formats can be identified for the standardized ingestion of data from multiple security components: 

* OCSF - Open Cybersecurity Schema Framework (developed by Splunk and AWS)  
* ECS - Elastic Common Schema (developed by Elastic) 
* OHDF - OASIS Heimdall Data Format (developed by MITRE). 

Using these formats, both on the producer and the consumer side make it possible to receive events from different sources and technologies and store them consistently for later analysis. It also avoids developing a specific integration for a specific product 

#### 4.2.2 Orchestration  

To facilitate orchestration, OXA will leverage the standardization work of CACAO (Collaborative Automated Course of Action Operations for Cyber Security).  

Indeed, CACAO members have developed a standard for the implementation of playbook  templates in cybersecurity operations. By defining a sequence of actions that can be executed for each kind of playbook and structured in a machine-readable format, CACAO simplifies and improves the orchestration process. 

#### 4.2.3 Automation 

Automation is the use of software to create repeatable orders and workflows, with the goal of reducing human intervention or replacing it with automated computer systems. 

Automation can be used to enrich, accelerate or replace human-led actions and give them more scope or efficiency (in particular by proposing the possibility of automating complex orchestrated intervention plans). 

As part of the OXA framework, OXA members are invited to look at OpenC2. Open C2 is a standardized language for sending commands and control messages to technologies that provide or support cyber defense.  

Knowing that many products already have their API to interact with the rest of the world, OXA project has released an additional tool named Meshroom. Meshroom allows each product editor to describe its capabilities and share it publicly so that other solutions know how to leverage it. 

#### 4.2.4 Cyber Intelligence Sharing (CTI) 

In order to better disseminate threat intelligence within an organization's security components, OXA will rely on two complementary CTI standards: STIX and TAXII. 

STIX (Structured Threat Information eXpression) is a standardized and structured language for representing cyber threat information, and in particular indicators of compromise (IOCs) obtained by threat intelligence. 

TAXII (Trusted Automated eXchange of Indicator Information) is a protocol designed to facilitate the exchange of CTI-type information, formatted in STIX. 

The use of these standards helps promote a globalized approach to threat intelligence. By adopting STIX / TAXII, OXA aims to promote a maximum interoperability between detection and response systems, allowing for smooth communication of threat indicators. 

One simple but smart approach in OXA consist in sharing the centralized threat intelligence filtered by technical categories that match product interests. 


#### 4.2.5 Setting up an API 

An API is an application programming interface that connects one software or service to another in order to exchange data and functionality. 

To meet the needs of the project, OXA is working on building an open API to allow the security components (let's call the Open XDR sensors) to benefit from all the Open XDR features on the back end.  

This open API should make it possible to govern all the interactions that can separate, on the one hand, the world of security products installed on or for the customer's environment, and on the other hand, the entire central environment and its components. This interface, when applied by security products, will allow them to ensure interoperability with any organization's back-end XDR environment. 

 
## 5. Review and Amendment of the Rule of Engagement 

This document may be revised by the OXA Governance Committee to reflect the changing needs of the project and the community. Changes will be communicated transparently to members. 

 

 
