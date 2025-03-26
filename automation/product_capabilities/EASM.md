# Product catagory
EASM stands for External Attack Surface Management  and plays an important role to identify how the digital environment of an organization is exposed.

Main capabilities will include:
- Discovery of external, digital assets
- Enumeration of software vulnerabilities
- Participate the remediation to exposures 

# Automation capabilities

| Action              |  Details | Target-Type | Arguments |
| :------------------ | :------- | :---------: | --------: |
|	discover  | discover asset within a generic starting point and bring knowledge as asset properties |[keyword, domain_name, ipv4_net, ipv6_net]|
|	scan  | enumerate vulnerabilities|[ipv4_net, ipv6_net, fqdn]|
|	assess | evaluate the criticality ot the asset  |[ipv4_net, ipv6_net, fqdn]|
|	query | query the actuator for its existing knowledge on a specific artefact |[ipv4_net, ipv6_net, fqdn]|

> When target-type is not provided, the consumer tries to guess the target based on its format 
