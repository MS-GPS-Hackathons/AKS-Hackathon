# Challenge 08 - AKS Monitoring

[< Previous Challenge](./Challenge-07-datavolumes.md) - **[Home](../README.md)** - [Next Challenge >](./Challenge-09-privatecluster.md)

## Introduction

Running a cluster without knowing what is going on inside of it is a show-stopper for any serious production deployment. It is imperative that we are familiar with operationalizing our Kubernetes clusters and having a full view into day to day running and error state alerts.

## Description

In this challenge you will learn how to view application logs and trouble-shoot errors. View performance metrics and identity bottlenecks.

- Find the logs for your application’s containers, using:
	- `kubectl`
	- Using the Kubernetes Dashboard
	- Notice how you can check the logs of any of your pods individually.
- Start a bash shell into one of the containers running on a pod and check the list of running processes
- Find out if your pods had any errors.
	- Figure out how to get details on a running pod to see reasons for failures.
- Implement Prometheus/Grafana **or** Azure Container Insights to be able to monitor cluster metrics
- You can access container logs via Azure Monitor

## Success Criteria

- Demonstrate and explain to your coach the usage of the kubectl commands: exec, describe, logs and explain
- Use kubectl to view logs for the containers running in your cluster.
- Demonstrate that you can login to a running container and issue bash commands.
- You can display cluster metrics graphically with Grafana or Container Insights
- You can show live container logs with Azure Container Insights

## Learning Resources

These docs might help you achieving these objectives:

- [Azure Monitor for Containers](https://docs.microsoft.com/azure/azure-monitor/insights/container-insights-overview)