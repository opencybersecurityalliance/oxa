
<p align="center">
<img src="https://github.com/opencybersecurityalliance/oxa/assets/145455635/639260e4-c101-47b2-bf95-302d4ad73f21" width="50%">
</p>

Data ingestion refers to the process of collecting data from different sources speaking different languages, translating it into a common language and storing it on a destination node, where it can be levered for further analysis or hunting.

In practical terms, this means receiving information from a variety of security-related heterogenous sensors,  and storing it on a unified system.


# Rationale

OXA framework considers the ingestion process is fostered when four different issues are solved:
- the sensor produces events that are created using structured content, ideally a standard
- the produced events are conveyed (from the sensor to the analytics) in a transport protocol, ideally a standard 
- the incoming events (at the analytics side) are normalized as structured content, ideally a standard
- the normalized events are stored on a system that can allow scalability and accessibility, ideally a standard


# Ingestion stages

**On the sensor stage**, OXA does not intend to replace existing standards. Several of them already exist and perform well :
- [OpenTelemetry](https://opentelemetry.io/) (which has integrated [Elastic Common Schema - ECS](https://github.com/elastic/ecs/tree/main))
- [Open Cybersecurity Schema Framework - OCSF](https://schema.ocsf.io/)
- [Common Event Format - CEF](https://www.microfocus.com/documentation/arcsight/arcsight-smartconnectors-8.3/cef-implementation-standard/Content/CEF/Chapter%201%20What%20is%20CEF.htm)
- [OASIS Heimdall Data Format - OHDF](https://github.com/oasis-tcs/ohdf)  
- [Intrusion Detection Message Exchange Format - IDMEF](https://github.com/IDMEFv2)
OCSF, OpenTelemetry/ECS, CEF have a large community adoption.
**OCSF, OpenTelemetry/ECS are the preferred OXA choices for sensor solutions, considering next stages and current community adoption**

**On the transport stage**, Syslog (and its secure evolutions) has been an historical solution  to distribute log on other systems. 
Modern log transport relies more and more on HTTP. It can then be used in two ways:
- The sensor-producer will push the events to the analytics-consumer
- The analytics-consumer will pull the events from the sensor-producer-management console 
**OXA has no preference on the transport being used**

**On the normalization stage**, when the incoming events are directly structured in a rich format it will allow valuable cybersecurity use cases:
- turnkey enrichment, 
- real-time detection analytics, 
- complex queries for future hunting activities
For that, **OCSF and OpenTelemetry/ECS have a real advantage because they both use a rich schema. OXA recognizes these two solutions as the preferred ones for an analytic solution**.  

**On the storage stage**, two main approaches can pretend to compete:
- the first one relies on Elasticsearch, as a  scalable data store and distributed search engine. Elasticsearch is relevant for incoming events structured as OpenTelemtry/ECS
- the second one relies on S3 from AWS, now widely adopted as as de-factor distributed object storage. S3 is very relevant for incoming events structured as OCSF or any security solution activated into a AWS ecosystem. 
**OXA has no preference on the storage being used for analytics solution**


# Conclusion

For a relevant ingestion capability, **two Frameworks are preferred: OCSF and OpenTelemetry/ECS**.
OXA brings some resources to accelerate the use of OCSF and/or OpenTelemetrECS
 

