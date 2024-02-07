---
name: EV Charging Platform
tools: [AWS, Kubernetes, Docker, Terraform, CDK, Python, Gherkin, Azure DevOps, Grafana]
image:
description: Multinational Energy Provider
---

# The Engagement

My time on this engagement was spread across multiple teams, though they were all related to the EV charging platform, 
either directly within the core EV charging platform infrastructure team, or within orbiting teams. My roles were always 
relating to the Cloud infrastructure. I’ll talk through my various roles and how they tied into the core EV charging 
platform.

## Core Platform Team
The core platform was composed of multiple microservices hosted on a Kubernetes EKS cluster, following a micro frontend 
architecture. My role within the team entailed managing, maintaining and improving the infrastructure as well as 
supporting application teams in integrating their services to the platform.

## DataHub Team
As the name implies, the DataHub team was charged with developing a central platform for managing data from multiple 
sources, specifically data relating to the EV charging platform. My role in this team was to help them architect and 
develop their platform on AWS using an event driven architecture. I was specifically involved with advising on best 
practices for an event driven architecture, defining their coding standards, developing their IaC utilising AWS CDK, 
their CI/CD processes utilising Azure DevOps, and their testing strategy.

## R&D Team
The R&D, or more specifically, the part of the R&D that I was working with, were in charge of creating services to 
simulate and test EV charging points and the way in which they would integrate to the core EV charging platform. This 
was composed of a number of applications, which needed to be hosted on AWS. My role was to architect the infrastructure 
solution on AWS, defining their coding standards, developing their IaC utilising AWS CDK, their CI/CD processes 
utilising Azure DevOps, and their testing strategy.
