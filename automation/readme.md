<p align="center">
<img src="https://github.com/opencybersecurityalliance/oxa/assets/145455635/4650ee62-a470-42d7-a337-5a781a988274" width="50%">
</p>

Automation consists in the use of software or tools to create replicable commands and workflows, with the aim of reducing human intervention or substituting it with automated computing systems.

In OXA framework, automation is used to enrich, accelerate or replace human actions and provide greater scope or efficiency (notably by proposing the possibility to automate complex orchestrated response plans).



# Rationale

OXA framework considers that the automation process is fostered when different issues are solved:
- automation is about actioning capabilities and the best way to define what an actions is is through a standard,
- sensors (cybersecurity products more globally) can be automated when they have these action capabilities,
- when a standard cannot be enforced on products, at least 'action grips' can be leveraged,
- a directory of available automation capability exist to address the ecosystem

OXA addresses these issues by combining existing approaches and providing new ones!

![](../resources/automation.svg)

# Automation related Standards 

The only standard that is focused on cybersecurity automation is OpenC2 by OASIS. Two main documents can be used as reference on OpenC2
- [OpenC2 Architecture](https://docs.oasis-open.org/openc2/oc2arch/v1.0/oc2arch-v1.0.html)
- [OpenC2 Language Specification](https://docs.oasis-open.org/openc2/oc2ls/v1.0/oc2ls-v1.0.html)

Although OpenC2 could be defined as an ultimate goal in automation, the industry adoption is not generalized. Instead of having a widely adopted automation library using OpenC2, SOAR products paved the way of automation market and restrained users in their proprietary environments. The result lead to a very disparate ecosystem where each point solution develop (or not) some API endpoints that can be triggered to activate some automation capabilities.
Even if the evolution of mesh architecture of cybersecurity solutions did not leverage the OpenC2 architecture until now, the language specification can still be leveraged easily to be used as an interface between product A and product B.

**OXA promote the OpenC2 language in a way that actions can be engaged on point solutions**
 

# Technology profiles
Market analyst job is to define categories of product and then, on one side help companies to define which category is great for them, and on the other side to help vendors to explain which critical capabilities they need.
Wether you like or not, it allows to define an technological landscape.

If we consider categories of products that are related to Security Operations, we can list some of them and define what their critical automation capabilities should be.

## Product categories and their automation capabilities
The product list is available in the ["product capabilities"](product_capabilities/) directory to be used as reference by cybersecurity editors.


# Ad hoc automation and Meshroom
If we consider some cybersecurity products can be activated with action grips available through their API (wether proprietary or compliant with OXA OpenAPI), a tool can be used to map the product category critical capabilities to these API endpoints.

This is the goal of [Meshroom](https://github.com/opencybersecurityalliance/meshroom) that aims to federating all cybersecurity interfaces into one single repository. This unlocks amazing possibilies such as uncurse the intergration hell of having NxN product integrations. 

Meshroom is a sub-part of OXA framework and is still very young but it can be massively used to federate cybersecurity products and optimize integrations teams time by 10x using a central repository.

Until then, OXA framework accepts contributions any vendors willing to define how they open their automation interfaces. 

**OXA strongly advocates cybersecurity products to use Meshroom to define their interface and the way they are willing to interact with the rest of the ecosystem**

# Central repository
A central repository of collective value (such as Automation capabilities of every products) need to located in a community space. As Meshroom is an OpenCyberAlliance project, it will serve as the central repository of these cybersecurity interfaces, including their automation scope.

**OXA considers the best way to leverage a federated repository of automation capabilities of any products will be the Meshroom Github repository** 

# Conclusion
OXA assumes the fact that the cybersecurity industry is diverse and far from having a common standard to have different products interact eachothers, including on automation side. To handle this reality, OXA framework comes along with a tool, dedicated to make integrations easier, create meshes between products and centralize the integrations for community use.



