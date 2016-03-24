# VNFaaS-Structure-Architecture-Description-and-Validation.
This repository contains further material related to the VNFaaS paper.

First the opensource codes (MJSIP http://www.mjsip.org/download/index.html and Little IMS https://github.com/ABoubendir/littleims) that have been used to analyze the functionnalities of IMS network functions.

By analyzing these network functions codes, we have realized that identifying the network functions that are involved in the Authentification and Authorization (AAA function) in IMS in order to extract it from them can be the first step.

We have then focused on P-CSCF, S-CSCF and HSS. Authentication and Authorization are tightly coupled in a way that we do not even distinguish two procedures. As explained in http://www.rfc-base.org/txt/rfc-3261.txt and http://www.rfc-base.org/rfc-4740.html. 

After this analysis, we have extracted all functionnalities related to Authentication and Authorization from these functions to rethink Authentication and Authorization in IMS to be perfomed by dedicated service components modeled as-a-Service based on the propsosed properties (stateless, cohesive, ...) 

Of course CSCF network functions and thus AAA fucntion do not respect as-a-Service properties (they are statefull, tightly coupled,..)

We build our business code for an Authentication function and another one for Authorization function respecting the properties when defining the service logic as explained in the paper. 

Then, we build the architectural design based on "as-a-Service" generic architecture relying on VCE Editor in VerCors platform (on Eclipse) for the architecture defenition and interfaces and behavior specifications. 

Then, 

The verification and validation of the VNFaaS components architecture and structure is made through VerCors Platform. 

VersCors platform is composed of different modules as shown in figure VerCors_platform_principles.png. The principles of VerCors are explained in file Architecture Verification and Validation over VerCors Modeling Platform.txt. 

The composition of Authentication-as-a-Service and Authorization-as-a-Service with interfaces is shown in figure Composition1.png. 

The validation of the architecture result is the Architecture Description Language (ADL) file: VNFaaS-composition.adl 

This architecture description is then implemented in ProaActive (https://github.com/scale-proactive/scale-proactive) 

Then we include 
