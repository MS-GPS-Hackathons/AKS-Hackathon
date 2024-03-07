# Coach Guide

## Introduction

Welcome to the coach's guide for this Hackathon. Here you will find links to specific guidance for coaches for each of the challenges.

**NOTE:** If you are a Hackathon participant, this is the answer guide. Don't cheat yourself by looking at these during the hack! Go learn something. :)

This hackathon is a mix of the three available “What the Hack” hackathons: [Intro to Kubernetes](https://github.com/microsoft/WhatTheHack/tree/master/001-IntroToKubernetes), [Advanced Kubernetes](https://github.com/microsoft/WhatTheHack/tree/master/023-AdvancedKubernetes) and [AKS Enterprise Grade](https://github.com/microsoft/WhatTheHack/tree/master/039-AKSEnterpriseGrade).

The [Intro to Kubernetes](https://github.com/microsoft/WhatTheHack/tree/master/001-IntroToKubernetes) hackathon includes an optional [lecture presentation](https://github.com/microsoft/WhatTheHack/blob/master/001-IntroToKubernetes/Coach/Lectures.pptx) that you may find useful delivering before starting the hackathon

The [Advanced Kubernetes](https://github.com/microsoft/WhatTheHack/tree/master/023-AdvancedKubernetes) hackathon also includes optional [lecture presentations](https://github.com/microsoft/WhatTheHack/tree/master/023-AdvancedKubernetes/Coach/Lectures) that you may find useful.

The hackathon solutions are references to the original WTH hackathons.

## Coach's Guides

- Challenge 00: **Prerequisites - Ready, Set, GO!**
	 - [WTH Intro To Kubernetes solution](https://github.com/microsoft/WhatTheHack/blob/master/001-IntroToKubernetes/Coach/Solution-00.md)
- Challenge 01: **Introduction To Kubernetes**
	 - [WTH Intro To Kubernetes solution](https://github.com/microsoft/WhatTheHack/blob/master/001-IntroToKubernetes/Coach/Solution-03.md)
- Challenge 02: **Your First Deployment**
	- [WTH Intro To Kubernetes solution](https://github.com/microsoft/WhatTheHack/blob/master/001-IntroToKubernetes/Coach/Solution-04.md)
- Challenge 03: **Operations and Monitoring**
	 - [WTH Intro To Kubernetes solution](https://github.com/microsoft/WhatTheHack/blob/master/001-IntroToKubernetes/Coach/Solution-11.md)
	 - [AKS Enterprise Grade solution](https://github.com/microsoft/WhatTheHack/blob/master/039-AKSEnterpriseGrade/Coach/Solution-03.md)
- Challenge 04: **Updates and Rollbacks**
	 - [WTH Intro To Kubernetes solution](https://github.com/microsoft/WhatTheHack/blob/master/001-IntroToKubernetes/Coach/Solution-07.md)
- Challenge 05: **Networking and Ingress**
	 - [WTH Intro To Kubernetes solution](https://github.com/microsoft/WhatTheHack/blob/master/001-IntroToKubernetes/Coach/Solution-10.md)
- Challenge 06: **Resiliency**
	 - [WTH Advanced Kubernetes Solution](https://github.com/microsoft/WhatTheHack/blob/master/023-AdvancedKubernetes/Coach/03-resiliency.md)
- Challenge 07: **Scaling**
	 - [WTH Advanced Kubernetes Solution](https://github.com/microsoft/WhatTheHack/blob/master/023-AdvancedKubernetes/Coach/04-scaling.md)
- Challenge 08: **Data Volumes**
	 - [WTH Advanced Kubernetes Solution](https://github.com/microsoft/WhatTheHack/blob/master/023-AdvancedKubernetes/Coach/07-data-volumes.md)
- Challenge 09: **AKS Network Integration and Private Clusters**
	 - [AKS Enterprise Grade solution](https://github.com/microsoft/WhatTheHack/blob/master/039-AKSEnterpriseGrade/Coach/Solution-02.md)
- Challenge 10: **Secrets and Configuration Management**
	 - [AKS Enterprise Grade solution](https://github.com/microsoft/WhatTheHack/blob/master/039-AKSEnterpriseGrade/Coach/Solution-04.md)
- Challenge 11: **AKS Security**
	 - [AKS Enterprise Grade solution](https://github.com/microsoft/WhatTheHack/blob/master/039-AKSEnterpriseGrade/Coach/Solution-05.md)
- (Optional) Challenge 12: **Helm**
	 - [WTH Advanced Kubernetes Solution](https://github.com/microsoft/WhatTheHack/blob/master/023-AdvancedKubernetes/Coach/02-helm.md)
- (Optional) Challenge 13: **GitOps**
	 - [WTH Advanced Kubernetes Solution](https://github.com/microsoft/WhatTheHack/blob/master/023-AdvancedKubernetes/Coach/05-gitops.md)
- (Optional) Challenge 14: **Service Mesh**
	 - [WTH Advanced Kubernetes Solution](https://github.com/microsoft/WhatTheHack/blob/master/023-AdvancedKubernetes/Coach/06-service-mesh.md)
	 - [AKS Enterprise Grade solution](https://github.com/microsoft/WhatTheHack/blob/master/039-AKSEnterpriseGrade/Coach/Solution-07.md)
- (Optional) Challenge 15: **Arc-Enabled Kubernetes and Arc-Enabled Data Services**
	 - [AKS Enterprise Grade solution](https://github.com/microsoft/WhatTheHack/blob/master/039-AKSEnterpriseGrade/Coach/Solution-08.md)


## Coach Prerequisites

This hack has pre-reqs that a coach is responsible for understanding and/or setting up BEFORE hosting an event. Please review the [What The Hack Hosting Guide](https://aka.ms/wthhost) for information on how to host a hack event.

The guide covers the common preparation steps a coach needs to do before any What The Hack event, including how to properly configure Microsoft Teams.

### Student Resources

Before the hack, it is the Coach's responsibility to download and package up the contents of the `/Student/Resources` folder of this hack into a "Resources.zip" file. The coach should then provide a copy of the Resources.zip file to all students at the start of the hack.


## Azure Requirements

This hack requires students to have access to an Azure subscription where they can create and consume Azure resources. These Azure requirements should be shared with a stakeholder in the organization that will be providing the Azure subscription(s) that will be used by the students.

- Attendees should have the “Azure account administrator” (or "Owner") role on the Azure subscription in order to authenticate their AKS clusters against their Azure Container Registries.  For more info: <https://docs.microsoft.com/en-us/azure/aks/cluster-container-registry-integration>

Attendees can use a shared Azure subscription.

## Suggested Hack Agenda

This hack is designed to be run as a full 4-day event, for a total of approximately 24 hours to complete all challenges. Different groups of students will complete the challenges at different paces based on their comfort level with Linux and/or using Command Line Interface (CLI) tools.  This is okay, and students should be encouraged to participate in this intro-level hack no matter what their experience level is.

Challenges from 12-15 are labeled as optional, if time permits and attendees area eager to learn more, they can complete these challenges as well, or give them to the attendees as homework.

### Challenges 0-4 and 8: 

These challenges are based on [Intro to Kubernetes hackathon](https://github.com/microsoft/WhatTheHack/tree/master/001-IntroToKubernetes)

### Challenges 5-7 and 12-14

These challenges are based on [Advanced Kubernetes hackathon](https://github.com/microsoft/WhatTheHack/tree/master/023-AdvancedKubernetes)

### Challenges 9-11 and 15

These challenges are based on [AKS Enterprise Grade hackathon](https://github.com/microsoft/WhatTheHack/tree/master/039-AKSEnterpriseGrade)

## Repository Contents

- `./Coach`
  - Coach's Guide and related files
- `./Coach/Solutions`
  - Solution files with completed example answers to a challenge
- `./Student`
  - Student's Challenge Guide
- `./Student/Resources`
  - Resource files, sample code, scripts, etc. meant to be provided to students. (Must be packaged up by the coach and provided to students at start of event)
