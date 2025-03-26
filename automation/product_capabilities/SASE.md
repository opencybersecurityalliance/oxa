# Product category
SASE stands for Security Access Service Edge and ensure the secure connection of users to the network.

Main capabilities will include:
- Ability to define a policy for network access
- Filtering of network communication up to the application layer and its content
- Detect malicious content
- Detect Data Theft behaviour 

# Automation capabilities

| Action              |  Details | Target-Type | Arguments |
| :------------------ | :------- | :---------: | --------: |
| query ||[account, hostname, ipv4, ipv6, fqdn, domainname||
| contain ||[account, hostname, ipv4, ipv6, domainname, fqdn]||
| allow ||[account, hostname, ipv4, ipv6, domainname, fqdn]||

> When target-type is not provided, the consumer tries to guess the target based on its format

