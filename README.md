# VNFaaS-Structure-Architecture-Description-and-Validation.
This repository contains further material related to the VNFaaS paper.

First the opensource codes (MJSIP and Little IMS) that have been used to analyze the functionnalities of IMS network functions.

By analyzing these network functions, we have realized that identifying the network functions that are involved in the Authentification procedure  in order to extract can be the first step.

(which is very coupled to authorization)

with a focus on P-CSCF, S-CSCF and HSS, and to understand the Authentification in IMS and identify the network functions that are involved in the authentification procedure (which is very coupled to authorization) to allow to extract it and rethink Authentication and Authorization in IMS to be perfomed by dedicated service components modeled as-a-Service. 

Of course

The verification and validation of the VNFaaS components architecture and structure is made through VerCors Platform. 

VersCors platform is composed of different modules as shown in figure VerCors_platform_principles.png. The principles of VerCors are explained in file Architecture Verification and Validation over VerCors Modeling Platform.txt. 

The composition of Authentication-as-a-Service and Authorization-as-a-Service with interfaces is shown in figure Composition1.png. 

The validation of the architecture result is the Architecture Description Language (ADL) file: VNFaaS-composition.adl 

This architecture description is then implemented in ProaActive (https://github.com/scale-proactive/scale-proactive) 

