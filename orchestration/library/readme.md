
# Overview

This library provides CACAO playbooks that can be used to provide orchestration capabilities.

CACAO stands for Collaborative Automated Course of Action Operations.
It's a schema and taxonomy for cyber security playbooks.

CACAO classified playbooks into different categories
- attack playbooks
- detection playbooks
- engagement playbooks
- investigation playbooks
- mitigation playbooks
- notification playbooks
- prevention playbooks
- remediation playbooks

The example below details how a mitigation playbook can ask a network operator to block a malicious MAC address on a switch.




# Example
``` 
{
  "type": "playbook",
  "playbook_types":["mitigation"],
  "spec_version": "cacao-2.0",
  "id": "playbook--fe85f68d-1960-4596-96a2-228113e143cf",
  "name": "Bad MAC Address",
  "description": "This playbook addresses a malicious MAC address, illustrating an action step, command, and agent/target.",
  "playbook_processing_summary": {},
  "created_by": "identity--351b1469-64b4-4778-8d93-f7949a88990d",
  "created": "2023-02-19T01:09:00.000Z",
  "modified": "2023-02-19T01:09:00.000Z",
  "workflow_start": "start--fa16a4e9-e6b9-4658-b464-ca1632ff57f4",
  "workflow": {
    "start--fa16a4e9-e6b9-4658-b464-ca1632ff57f4": {
      "type": "start",
      "description": "Start example playbook.",
      "on_completion": "action--6398eb05-3eb8-43f5-87d3-f24e07492a41"
    },
    "action--6398eb05-3eb8-43f5-87d3-f24e07492a41": {
      "type": "action",
      "name": "Block MAC address",
      "description": "This command blocks a MAC address on a switch.",
      "commands": [{
        "type": "ssh",
        "command": "Switch(conf)#mac address-table static 3467.0933.341c vlan X drop"
      }],
      "agent": "individual--75baba7d-a198-4c5c-805c-af616b4f7a31",
      "targets": ["security-category--3c1daf98-7e22-4e0c-bb8c-6bd78159ca5d"],
      "on_completion": "end--116cdac5-63f1-4d8f-b3a8-e5667936e9b6"
    },
    "end--116cdac5-63f1-4d8f-b3a8-e5667936e9b6": {
      "type": "end",
      "description": "End of example playbook."
    }
  },
  "agent_definitions": {
    "individual--75baba7d-a198-4c5c-805c-af616b4f7a31": {
      "type": "individual",
      "name": "Network Admin",
      "description": "The admin who responds to an alert by configuring a switch."
    }
  },
  "target_definitions": {
    "security-category--3c1daf98-7e22-4e0c-bb8c-6bd78159ca5d": {
      "type": "security-category",
      "name": "Switch",
      "category": ["switch"]
    }
  }
}
```


# Resources

Some resources already provide CACAO usecases or explanations:

- https://docs.oasis-open.org/cacao/security-playbooks/v2.0/security-playbooks-v2.0.html
- https://www.signalscorps.com/blog/oasis-cacao-101-introduction/ 
- https://github.com/oasis-tcs/cacao/tree/master/Examples/CACAO-2.0

Some resources provides playbooks that are interesting (but not using CACAO) 
- https://github.com/Azure/Azure-Sentinel/tree/master/Playbooks
- https://github.com/SEKOIA-IO/Community/tree/main/playbooks/templates


