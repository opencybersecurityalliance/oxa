
![Ingestion for OXA](https://github.com/opencybersecurityalliance/oxa/assets/145455635/639260e4-c101-47b2-bf95-302d4ad73f21)

Data ingestion refers to the process of collecting data from different sources speaking different languages, translating it into a common language and storing it on a destination node, where it is ready to be analyzed and used. 

In practical terms, this means bringing together information from a variety of security sensors that do not necessarily communicate with each other and centralizing them in a unified system. 

To do so, OXA will rely on a transformer stage  and leverage best practices formats used for ingestion. To date, three different formats can be identified  for ingesting data from multiple security components : 
- ECS - Elastic Common Schema (developed by Elastic) 
- OCSF - Open Cybersecurity Schema Framework (developed by Spunk and AWS)
- OHDF - OASIS Heimdall Data Format (developed by MITRE)

These formats allow to receive  events originating from different sources and technologies and store them coherently for further analysis. 

