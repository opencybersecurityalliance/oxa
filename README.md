# OXA - Open XDR architecture

## Overview

OXA is an Open [Cybersecurity Alliance (OCA)](https://opencybersecurityalliance.org) project. 
The goal is to facilitate interactions between security products, using open standards and APIs.
This sounds particularly suited to define the architecture of an ideal eXtended Detection and Response approach.



## Project genesis

XDR is a direction given for security industry but without standardized guidelines.
X stands for eXtended, meaning that ingesting and interacting with products should be possible at the industry level, not with specific vendor-to-vendor connector.

D stands for Detection and detection is mostly applied in central areas or specific components using a licenced based threat-intel repository. Sharing efficiently threat intelligence between components could be a game changer to accelerate the response stage

R stands for Response and today it’s not possible to ask orders to security components without having to translate actions into their proprietary langage. An open “dictionnary” used to map generic/proprietary actions would help to have Response at scale everywhere.

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


## Contributing
We are thrilled you are considering contributing! We welcome all contributors. Guidelines for contributing will come soon.

## Join us on slack

[Click here](https://docs.google.com/forms/d/1vEAqg9SKBF3UMtmbJJ9qqLarrXN5zeVG3_obedA3DKs/viewform?edit_requested=true) and fill out the form to receive an invite to the Open Cybersecurity Alliance slack instance, then join the #oxa channel, to meet and discuss usage with the team.

## Documentation
Documentation related to OXA is maintained in the OCA OXA GitHub respository. A dedicated website will be available soon to describe the approach visually.
