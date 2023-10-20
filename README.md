
![OXA logo](https://github.com/opencybersecurityalliance/oxa/blob/main/OXA%20logo3.jpg)
OXA - Open XDR architecture



# Overview

OXA is an [Open Cybersecurity Alliance (OCA)](https://opencybersecurityalliance.org) project. 
It stands for **Open XDR Architecture**.
It notably provides a library of mapping files so that every cybersecurity product can speak to another one. If everyone does not share the same language, at least, let's have dictionnaries!

# The Goal
The goal is to facilitate interactions between security products, using open standards and APIs and with a special focus on Detection and Response.
This project aims to define the architecture of an ideal eXtended Detection and Response approach.

## Benefits for users
- Industry best practices are available as playbooks
- Ability to plug solutions easily without waiting vendor integration
- CTI-enabled products

## Benefits for customers
- No vendor lock-in 
- Valuation of the existing IT environment
- SOC ready in a day

## Benefits for service providers
- Change a SOC stack easily
- Can mutualize industry-based playbooks
- Can provide cybersecurity services for smaller customers 

## Benefits for cybersecurity vendors
- Only one inbound and one outbound mapping instead of a connector with every vendor of the industry
- Actionability of vendor's product automatically
- CTI-powered vendor's product automatically

# In a nutshell
![OXA](https://github.com/opencybersecurityalliance/oxa/assets/145455635/0a193f6b-532e-4086-9b71-067a8cad441b)

OXA is a common set of libraries and interfaces that allows cybersecurity industry to interact


# Project genesis

XDR is a direction given for security industry but without standardized guidelines.
- X stands for eXtended, meaning that ingesting and interacting with products should be possible at the industry level, not with specific vendor-to-vendor connectors.
- D stands for Detection and detection is mostly applied in central areas or specific components using a licenced based threat-intel repository. Sharing threat intelligence efficiently between components could be a game changer to accelerate the response stage
- R stands for Response and today it’s not possible to launch commands on security components fron another product without having to translate actions into their proprietary langage. An open “dictionnary” used to map generic/proprietary actions would help to have Response at scale everywhere.

Combining these topics as a generic approach leads to an open architecture. This architecture could then be used, partially or entirely by editors to have their solutions be XDR-ready almost instantly and benefit from a global threat sharing.
The output of this project are open source repositories to accelerate market adoption and industry implementation.

# Standards use

OXA relies on:
* STIX/TAXII for threat intelligence dissemination along security components
* OpenC2 for ordering generic actions that shoulg be executed on security components
* CACAO for defining the community orchestrated best practices on response strategies
* ECS/OCSF for ingesting logs from security components
* A open REST/API to create an interface beetween security products and the XDR back-end side
 
# Licence

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at
http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.


# Contributing
We are thrilled you are considering contributing! We welcome all contributors. Guidelines for contributing [can be found here](./CONTRIBUTING.md).

## Join us on slack

[Click here](https://join.slack.com/t/open-cybersecurity/shared_invite/zt-1jsgt1053-oYsfBPXXChhbRO4JO5Xo1A) and fill out the form to receive an invite to the Open Cybersecurity Alliance slack instance, then join the #oxa channel, to meet and discuss usage with the team.

# Documentation
Documentation related to OXA is maintained in the OXA GitHub respository of OpenCybersecurityAlliance. A dedicated website will be available soon to describe the approach visually.
