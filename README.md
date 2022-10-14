# Workshop - Deploy F5 BIG-IP Failover via F5 Cloud Solution Templates v2 in AWS

_____
**Disclaimer: This workshop is a community owned initiative intended to educate F5 BIG-IP addicts how to leverage F5 Cloud Solutions Templates. This workshop does **NOT** come with F5 support and when deployed in your own environment use it at your own risk.**
_____

## Introduction
The following workshop goes through the use of **Cloud Solution Templates v2 (CSTv2)** to deploy BIG-IPs in AWS. F5 Cloud Solution Templates v2 are available for Cloud Solution Providers like: [AWS](https://github.com/F5Networks/f5-aws-cloudformation-v2), [Azure](https://github.com/F5Networks/f5-azure-arm-templates-v2) and [Google Cloud Platform (GCP)](https://github.com/F5Networks/f5-google-gdm-templates-v2). These templates are developed by F5 to deliver an easy way to deploy and implement F5 BIG-IP solutions in the mentioned public cloud provider environments.

## CSTv1 vs. CSTv2
Before the introduction of CSTv2 there was CSTv1. CSTv1 are in maintenance mode and being replaced by CSTv2 and therefore it is strongly advised to use CSTv2 instead of v1.

CSTv2 have been designed to improve the user experience with fewer templates, simplify full-stack deployments, enable customization via a new modular nested/linked architecture. The templates have been tested and verified to work as-is and are intended to provide reference deployments of F5 BIG-IP Virtual Editions.

Another reason to start using CSTv2 is because they use BIG-IP [Runtime-init](https://github.com/F5Networks/f5-bigip-runtime-init) which allows to:
- Include support to leverage [F5 Automation Toolchain](https://www.f5.com/pdf/products/automation-toolchain-overview.pdf);
- Renders secrets from public cloud vaults;
- Renders runtime variables from cloud metadata services.


## How to use this workshop
For invited student an F5 UDF lab environment will be available which includes access to an AWS cloud environment and all needed facilities.
When you don't have an F5 UDF lab available you can still leverage the content. Use your own environment to install the needed packages and explore by using this workshop.

The pre-requistes are:
* Owner of an AWS account
* AWS CLI installed
* Git installed
* Visual Studio Code installed
* F5 VSC extension installed

## What you will learn
How to use CSTv2 to deploy BIG-IP Failover design in AWS when a **network already exists** AKA 'existing stack' and customize the template for local usage.

Tasks to deploy are:

* Learn AWS basics
* Manually create a VPC, affiliated networking components and a test application
* Use CSTv2 'existing network' to deploy BIG-IP

The mix between manually configuring AWS components and the use of CloudFormation Templates (CFTs) make that one will better understand the deployed objects and the relationship between each other.

--Happy Learning--

**********************************
## Table of Contents
**********************************

**[0. Getting Started](docs/0_Getting_Started.md)**

**[1. Deploy VPC and More](docs/1_Setup_the_VPC_and_More.md)**

**[2. Deploy BIGIPs with CSTv2](docs/2_Deploy_BIG-IPs_with_CSTv2.md)**

**[3. Create F5 demo App](docs/3_Create_Demo_App.md)**

**[4. App Services Deploy and Test](docs/4_App_Services_Deployment.md)**

*********************************