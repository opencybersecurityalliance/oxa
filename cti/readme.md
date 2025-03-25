Threat Intelligence covers the process of collecting, processing, identifying and analyzing data about cyber threats in order to better understand them. 


<p align="center">
<img src="https://github.com/opencybersecurityalliance/oxa/assets/145455635/f82aee53-22fa-4d7f-83bd-b31f54ca9ae4" width="50%">
</p>





# Rationale

Threat Intelligence enables organizations to make faster, smarter and better-informed security decisions. It encourages proactive, rather than reactive, behavior in the ongoing fight against cyber-attacks.

In order to better **disseminate threat intelligence along security components within an organization scope** , OXA relies on two complementary CTI standards : STIX & TAXII. 
- [STIX](https://docs.oasis-open.org/cti/stix/v2.1/stix-v2.1.html) (Structured Threat Information Expression) is a standardized, structured language for representing information on cyber threats including indicators of compromise (IOCs) that can be leveraged by technical tools.
- [TAXII](https://docs.oasis-open.org/cti/taxii/v2.1/taxii-v2.1.html) (Trusted Automated eXchange of Indicator Information) is a protocol designed to facilitate the exchange of CTI-type information, formatted in STIX.

These standards, when used correctly, enable corporate security teams to be informed about the attacks they are most likely to suffer, so they can adapt and respond to them as quickly and effectively as possible. 
However, it's broadly observed that existing threat intelligence into an organization is not made actionable enough for this same organization. 
OXA aims at leveraging TAXII for the distribution of a robust CTI that can feed different security components, each of them being interested in different kinds of threat intelligence artifacts.

![](../resources/cti.svg)


# Technology Profiles 

## Indicators and observables

In STIX model, indicators are using a pattern field that correspond with an observable element. This pattern can be used by a system as a technical mean to detect the indicated threat locally.
Some patterns will be relevant for some cybersecurity product (ie ipv4-addr is interesting for a network device and may be not for a file monitoring solution)

## Profiles 

OXA propose to map the need of cybersecurity products into different technology profiles and to associate specific patterns of indicators to these profiles.
The list of profile capabilities for CTI consumption is:
- identity: solutions that provide features based on identity
- malware:  solutions that provide features based on malware handling
- system:  solutions that provide features based on system activity
- network:  solutions that provide features based on network activity

# Contributions

OXA lists CTI solutions that can provide this capability. This should be available as a feed URL or as an OXA OpenAPI endpoint



