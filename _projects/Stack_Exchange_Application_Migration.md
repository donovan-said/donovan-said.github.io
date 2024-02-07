---
name: Application Migration
tools: [AWS, Terraform, Ansible, Vault, PostgreSQL, Python, behave, Jenkins]
image:
description: Stock Exchange
---

# The Engagement

Throughout this engagement I wore multiple “hats”, specifically as the Cloud Architect, Technical Lead and Project 
Manager. The objective of this engagement was to re-platform a core financial application from on-prem to AWS. The 
application itself served multiple financial markets, and had to be able to have multiple instantiations of itself 
which operated independently, which had to be taken into consideration when architecting and developing this solution.

As part of this re-platform we took the opportunity to modernise the infrastructure to allow automatic scaling of 
servers and databases, as well as utilising IaC with Terraform, Secret Management with Vault, Application Configuration 
with Ansible, and CI/CD with Jenkins and Bitbucket for our VCS.

The application itself was refactored to handle scaling and the utilisation of Read Replicas in AWS’ database service 
RDS. We also had to migrate the database from Oracle hosted on-prem to PostgreSQL hosted on RDS, which required 
significant refactoring SQL scripts.

In addition to the above, we were able to implement a modern application release lifecycle which reflected the 
accelerated pace of deployments on Cloud platforms.