# Challenge 05 - Resiliency

[< Previous Challenge](./Challenge-04-ingress.md) - **[Home](../README.md)** - [Next Challenge >](./Challenge-06-scaling.md)

## Introduction

Resiliency is the ability to recover quickly from issues.  For Cloud Native applications, we want to rely upon automation when possible.  We will add Readiness and Liveness Probes to our existing containers and validate them

## Description

For this challenge, we will use <https://github.com/stefanprodan/podinfo> application since it exposes a number of Web API's for interacting with the container.  

- Provision the Podinfo application in your cluster
- **NOTE:** Sample YAML files to get you started can be found in the `/Challenge-05/` folder of the `Resources.zip` package provided by your coach.
- Ensure you have multiple replicas of podinfo running
- Update the Liveness Probe of your deployment to use `/healthz`
- Update the Readiness Probe of your deployment to use `/readyz`
- Force the Readiness Probe to fail for a specific instance
    - HINT: look through some of the APIs in the [repo README](https://github.com/stefanprodan/podinfo) and execute ([exec](https://kubernetes.io/docs/reference/kubectl/generated/kubectl_exec/)) in a specific pod that you want to fail.

## Success Criteria

- Before disabling the readiness probe, when you refresh the podinfo page, the hostname should rotate through each of the running pods.
- After disabling the response to the readiness probe, one of the hostnames should no longer be in the rotation
- After disabling the response to the readiness probe, Use `kubectl` to verify that one pod is no longer in the rotation

## Optional challenge

- Get all pods back to a ready state
- After getting all pods in the ready state, use `kubectl` to verify all pods are ready

## Hints

1. [PodInfo web API](https://github.com/stefanprodan/podinfo)
1. [Liveness, Readiness and Startup Probes](https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/)
1. [cURL manual](https://curl.haxx.se/docs/manual.html)
1. [Kubernetes probes](https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle/#container-probes)
