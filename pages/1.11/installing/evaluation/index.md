---
layout: layout.pug
navigationTitle:  Evaluation
title: Evaluation
menuWeight: 10
excerpt: Installing DC/OS for evaluation on cloud or on-premise infrastructure
---

This page supports both DC/OS OSS (default) and DC/OS Enterprise installation methods. You can evaluate the installation of DC/OS cluster based on your requirements.

**Note:** The following installation methods are not officially supported by Mesosphere, but are supported by the DC/OS community. Contact the [mailing list](https://groups.google.com/a/dcos.io/forum/#!forum/users) or [Slack channel](http://chat.dcos.io/?_ga=2.226911897.58407594.1533244861-1110201164.1520633201) for community support.

# Types of installation methods

Use the following installation methods based on your requirement.
 
## Cloud Installation 
The cloud installation method is used for fast demos and POCs. 

DC/OS CloudFormation templates are intended for reference only and are not recommended for production use, due to the following limitations:
- CloudFormation does not allow for coordinated zero-downtime in-place updates within Auto Scaling groups.
- CloudFormation does not allow for automated zero-downtime replacement of Auto Scaling groups.
- Replacing DC/OS agent nodes requires manual data migration of local storage volumes for stateful services.
- Updates of DC/OS on AWS CloudFormation have not been automated, validated, or documented.
- Modified CloudFormation templates are not supported by Mesosphere, Inc.

The following methods are used to install DC/OS:
- Provision DC/OS on Amazon Web Services (AWS): Install DC/OS cluster on Amazon Web Services (AWS) by using the DC/OS templates on AWS CloudFormation. 
- Provision DC/OS on Azure: Install DC/OS cluster on Azure by using the Azure Resource Manager templates.
- Provision DC/OS on Google Cloud Platform (GCE): Install DC/OS cluster on Google Compute Engine (GCE) by using installation scripts. Upgrades are not supported with this installation method.

**Note:** The recommended way to install production ready DC/OS that can be upgraded in-place is to use the [production installation](/1.11/installing/production/deploying-dcos/installation/) method.

## On-premise Installation 
The on-premise installation uses various methods to install DC/OS. 
