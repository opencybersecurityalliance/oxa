# Product catagory
EDPP stands for Endpoint Protection Platform whereas EDR stands for Endpoint Detection and Response. Both are largelly included into the same product category. They are widely deployed on organization to protect against different kind of malware

Main capabilities will include:
- Scan a device
- Delete a file
- Quarantine files or programs
- Block or kill processes
- Isolate an endpoints
- Disconnec a user


# Automation capabilities

| Action              |  Details | Target-Type | Arguments |
| :------------------ | :------- | :---------: | --------: |
|	scan |	Initiate a scan for binaries classified as malicious. |||
|	list*	| Ask the ER actuator for a list of available features.|||
|	deny	| Deny a file or service from being executed on the endpoint. | [domain_name, file, ipv4_net, ipv6_net] ||
|	contain	| Isolate a device from communicating with other devices on a network, quarantine a file. | [device, file, account*]||
|	allow	| Un-isolate a previously isolated device or target.| [device, domain_name, file, process, ipv4_net, ipv6_net]||
|	start	| Initiate a process, application, system, or activity. |  [file]||
|	stop	| Halt a system or end an activity. | |device, process, service] ||
|	restart	| Restart a device, system, or process. | [device, process] ||
|	set	| Change a value, configuration, or state of a managed entity (e.g., registry value, account). |||
|	update	| Instructs the Actuator to retrieve, install, process, and operate in accordance with a software update, reconfiguration, or other update. |||
|	create	| Add a new entity of a known type (e.g., registry entry, file). |||
|	delete	| Remove an entity (e.g., registry entry, file). |||
| retrieve* | Retrieve telemetry of an agent on a timeframe | [file, process, account*, domain_name, ipv4_net, ipv6_net]|  [start_time, stop_time, duration] |
| query* | query the ER actuator for its existing knowledge on a specific artefact |||


> * evolution proposal compared with the [OpenC2 EDR actuator profile](https://github.com/oasis-tcs/openc2-ap-er/blob/working/oc2edr.md) for better alignment with product critical capabilities or simplicity
> When target-type is not provided, the consumer tries to guess the target based on its format 
