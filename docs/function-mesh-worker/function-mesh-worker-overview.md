---
title: Function Mesh Worker service overview
category: function-mesh-worker
id: function-mesh-worker-overview
---

This document gives a brief introduction into Function Mesh Worker service.

# What is Function Mesh Worker service

Function Mesh Worker service is a plug-in for Pulsar. It is similar to Pulsar Function Worker service but uses Function Mesh operators to schedule and run functions. Function Mesh Worker service enables you to use the [`pulsar-admin`](https://pulsar.apache.org/docs/en/pulsar-admin/) or [`pulsarctl`](https://docs.streamnative.io/pulsarctl/v2.7.0.7/) CLI tools to manage Pulsar functions and connectors in Function Mesh.

# How Function Mesh Worker service works

The following figure illustrates how Function Mesh Worker service works with Pulsar proxy, converts and forwards function and / or connector admin requests to the Kubernetes cluster. The benefit of this approach is that you do not need to change the way you create and submit functions and / or connectors.

![Function Mesh Workflow](./../assets/function-mesh-workflow.png)

# Version matrix

This table lists the version mapping relationships between Function Mesh and Function Mesh Worker service.

| Function Mesh | Function Mesh Worker service |
| --- | --- |
| v0.1.9 | <br />- v2.9.1 .x (v2.9.1.1-v2.9.1.2) <br />- v2.8.2.x (v2.8.2.0- v2.8.2.1 v2.8.2.2) <br />- v2.8.1 x (2.8.1.25-v2.8.1.26, v.2.8.1.28-v2.8.1.30)|
