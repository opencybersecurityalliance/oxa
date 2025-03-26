An API is an Application Programming Interface that connects a piece of software or a service to another in order to exchange data and features.

<p align="center">
<img src="https://github.com/opencybersecurityalliance/oxa/assets/145455635/411eeec6-fcf1-4185-ba37-88da4b3bb9c6" width="50%">
</p>

Hence, OXA is working on building an OpenAPI in order to allow security components (let’s name them Open XDR "Front End" sensors) to benefit from all Open XDR "Back End" side fonctionnalities delivered by Security Analytics component. This Open API spec allows to foster interactions between the world of security products installed into an organization and the a central analytics product serving this API. This interface, once enforced by security products, will enable them to guarantee their interoperability between "front-end" and "back-end" XDR environment of any organization.

To date, there is no existing international standard to respond to such needs. The OXA Framework propose this OpenAPI spec to be used globally for XDR interactions. 



# Rationale

OXA framework considers the interaction between cybersecurity products is fostered:
- either when products team have developped integrations
- or when product A can guess what product B is supposed to do because is complies with a defined API spec

![](../resources/openapi.svg)

OXA addresses these issues by providing [Meshroom](https://github.com/opencybersecurityalliance/meshroom), a tool to create integrations at scale and an OpenAPI spec that can be served either by front-end components or back-end components.



# OpenAPI spec

The OpenAPI Specification (OAS) is a standardized, language-agnostic format for describing RESTful APIs. It allows both humans and machines to understand an API's capabilities without accessing its source code or relying on external documentation. 

## On the front-end/sensor side 
Using the OpenAPI spec as a single source of trust to interact with the back-end/analytics side is a way forward to reach several objectives:
### Accelerate the creation of relevant workflow
When you know what you can be leveraged around you, you can create pre-defined workflows (for instance with this button, it will enrich my content thanks to my OXA peer)

### Being able to interact without knowing your peer
With an OpenAPI contract, the sensor can interact with an analytics component without having to develop a specific integration. Using the OXA compliance, the products SHOULD be able to speak, just leveraging the API


## On the back-end/analytics side 
Serving the OpenAPI spec in an environment of multiple product all compliant with OXA can be very convenient:

### Boost innovative technologies
By giving access to front-end side innovative product some capabilities that they do not fulfill themselves can help it to focus on its value without trying to integrate a global cybersecurity workflow.

### Ad-hoc environment
Every front-end component just have to enter some basic information, such as a server URL serving the central back-end OpenAPI and let's go, the environement is ready and cybersecurity workflow can flourish! 



