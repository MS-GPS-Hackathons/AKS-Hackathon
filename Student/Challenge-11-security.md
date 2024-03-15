# Challenge 11 - AKS Security

[< Previous Challenge](./Challenge-10-secrets.md) - **[Home](../README.md)** - [Next Challenge >](./Challenge-12-helm.md)

## Introduction

This challenge will cover the implementation of different security technologies in AKS.

## Description

You need to fulfill these requirements to complete this challenge:

- Make sure that the ingress controller is the only pod that can communicate to the Web pods
- Make sure that the API pods can only be accessed by the web pods or the ingress controller pods
- Make sure that no LoadBalancer services with a public IP address can be created in the Kubernetes cluster
- Add a user node pool to the cluster, if you hadn't configured it already and differentiate between user and system node pools
- Kubernetes administrators must authenticate to the cluster using their AAD credentials

## Success Criteria

- Participants can demonstrate that the network security controls are in place
- Application workloads are physically separated (in different nodes) from control plane workloads
- AAD authentication is required before being able to run any kubectl operation on the cluster

## Advanced Challenges (Optional)

- Make sure that the flag `--admin` is never required when using the command `az aks get-credentials`
- Make sure that access to the application over the ingress controller is encrypted with SSL, if you hadn't configured it already

## Learning Resources

These docs might help you achieving these objectives:

- [Policy in AKS](https://docs.microsoft.com/azure/governance/policy/concepts/policy-for-kubernetes)
- [Assigning Pods to Nodes](https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/#affinity-and-anti-affinity)
- [Taints and Tolerations](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
- [Kubernetes Network Policies](https://kubernetes.io/docs/concepts/services-networking/network-policies/)
- [Azure AD for authentication with Kubernetes RBAC](https://learn.microsoft.com/en-us/azure/aks/azure-ad-rbac?tabs=portal)

