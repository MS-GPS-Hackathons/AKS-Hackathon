# Azure Kubernetes Service Hackathon

## Introduction

Azure Kubernetes Service (AKS) simplifies the deployment of managed Kubernetes clusters in the Azure cloud. Kubernetes, an open-source system, automates the deployment, scaling, and management of containerized applications. 

In this hack you will solve a common challenge for companies migrating to the cloud. You will take a simple multi-tiered web app, containerize it, deploy it and manage it to an AKS cluster. Once the application is in AKS, you will learn how to tweak all the knobs and levers to scale, manage, secure and monitor your workloads.

This hackathon is a mix of the three available “What the Hack” hackathons: [Intro to Kubernetes](https://github.com/microsoft/WhatTheHack/tree/master/001-IntroToKubernetes), [Advanced Kubernetes](https://github.com/microsoft/WhatTheHack/tree/master/023-AdvancedKubernetes) and [AKS Enterprise Grade](https://github.com/microsoft/WhatTheHack/tree/master/039-AKSEnterpriseGrade). 


## Learning Objectives

The following topics will be covered.

-   Containerize an application
-   Deploy a Kubernetes cluster in Azure and deploy applications to it.
-   Understand key Kubernetes management areas: scalability, resiliency, upgrades and rollbacks, storage, networking, - curity, package management and monitoring
-   Deploy 3-tier application to AKS securely with very specific networking requirements.
-   Create and use Helm charts
-   Using Git as the Source of Truth for your cluster 
-   Learn about the features of a Service Mesh


## Challenges

- Challenge 00: **[Prerequisites - Ready, Set, GO!](Student/Challenge-00-prereqs.md)**
	 - Prepare your workstation to work with Azure, Docker containers, and AKS
- Challenge 01: **[Introduction To Kubernetes](Student/Challenge-01-cluster.md)**
	 - Install the Kubernetes CLI tool, deploy an AKS cluster in Azure, and verify it is running.
- Challenge 02: **[Your First Deployment](Student/Challenge-02-deploy.md)**
	 - Pods, Services, Deployments: Getting your YAML on! Deploy the "FabMedical" app to your AKS cluster.
- Challenge 03: **[Operations and Monitoring](Student/Challenge-03-monitoring.md)**
	 - Explore the logs provided by Kubernetes using the Kubernetes CLI, configure Azure Monitor or the managed Azure Prometheus/Grafana and build a dashboard that monitors your AKS cluster
- Challenge 04: **[Updates and Rollbacks](Student/Challenge-04-updates.md)**
	 - Deploy v2 of FabMedical to AKS via rolling updates, roll it back, then deploy it again using the blue/green deployment methodology.
- Challenge 05: **[Networking and Ingress](Student/Challenge-05-ingress.md)**
	 - Explore integrating DNS with Kubernetes services and explore different ways of routing traffic to FabMedical by configuring an Ingress Controller.
- Challenge 06: **[Resiliency](Student/Challenge-06-resiliency.md)**
	 - Explore resiliency by defining Readiness and Liveness probes
- Challenge 07: **[Scaling](Student/Challenge-07-scaling.md)**
	 - Flex Kubernetes' muscles by scaling pods, and then nodes. Observe how Kubernetes responds to resource limits.
- Challenge 08: **[Data Volumes](Student/Challenge-08-datavolumes.md)**
	 - Explore how to use and manage data volumes within your containers with persistent volumes (PV) and persistent volume claims (PVC)
- Challenge 09: **[AKS Network Integration and Private Clusters](Student/Challenge-09-privatecluster.md)**
	 - Deploy the application in an AKS cluster with strict network requirements
- Challenge 10: **[Secrets and Configuration Management](Student/Challenge-10-secrets.md)**
	 - Harden secret management with the help of Azure Key Vault
- Challenge 11: **[AKS Security](Student/Challenge-11-security.md)**
	 - Explore AKS security concepts such as Azure Policy for Kubernetes
- (Optional) Challenge 12: **[Helm](Student/Challenge-12-helm.md)**
	 - Explore how to use Helm to package your solution and services
- (Optional) Challenge 13: **[GitOps](Student/Challenge-13-gitops.md)**
	 - Explore how to use a Git repository as the source of truth for the desired state of your infrastructure and applications.
- (Optional) Challenge 14: **[Service Mesh](Student/Challenge-14-servicemesh.md)**
	 - Explore the service mesh capabilities like traffic management, resiliency, policy, security, strong identity, and observability to your workloads.
- (Optional) Challenge 15: **[Arc-Enabled Kubernetes and Arc-Enabled Data Services](Student/Challenge-15-arc-enabled-kubernetes.md)**
	 - Leverage Arc for Kubernetes to manage a non-AKS cluster, and Arc for data to deploy a managed database there

## Prerequisites

- Access to an Azure subscription with Owner access
   - If you don't have one, [Sign Up for Azure HERE](https://azure.microsoft.com/en-us/free/)
- [**Windows Subsystem for Linux (Windows 10-only)**](https://docs.microsoft.com/en-us/windows/wsl/install-win10)
- [**Azure CLI**](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli)
   - (Windows-only) Install Azure CLI on Windows Subsystem for Linux
   - Update to the latest
   - Must be at least version 2.5.x
- Alternatively, you can use the [**Azure Cloud Shell**](https://shell.azure.com/)
- [**Visual Studio Code**](https://code.visualstudio.com/)

## Contributors
- [Phanis Parpas](https://github.com/fparpas)
- [Piotr Filarski](https://github.com/PiotrFilarski)

## References

### Contributors from [WTH - Intro To Kubernetes](https://github.com/microsoft/WhatTheHack/tree/master/001-IntroToKubernetes)

- [Peter Laudati](https://github.com/fparpas)
- [Gino Filicetti](https://github.com/gfilicetti)
- [Israel Ekpo](https://github.com/izzymsft)
- [Sowmyan Soman Chullikkattil](https://github.com/sowsan)
- [Larry Claman](https://github.com/larryclaman)

### Contributors from [WTH - Advanced Kubernetes](https://github.com/microsoft/WhatTheHack/tree/master/023-AdvancedKubernetes)

- Tommy Falgout
- Kevin M. Gates
- Michelle Yang

### Contributors from [WTH - AKS Enterprise Grade](https://github.com/microsoft/WhatTheHack/tree/master/039-AKSEnterpriseGrade)

- Adrian Joian
- Gitte Vermeiren
- Jose Moreno
- Victor Viriya-ampanond
- Peter Laudati
- Pete Rodriguez
