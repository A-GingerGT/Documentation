---
title: Kubernetes Basics
---

## Command Line Tools


## Kubernetes Objects

In Kuberenetes, objects are organized in a hierarchal structure, similar to a Russian nesting doll.

```text
+---Cluster
|   +---Node
|   |   +---Pods
|   |   |   +---Containers
```

Containers are the smallest object in the structure, representing a program running on a virtual or physical
machine. 

The objects in Kubernetes are most easily defined using definition YAML files.

=== "Pods/Nodes"
    This is where the containers that run appications live. Conventionally, Pods contain a single application
    container, so scaling an application occurs by creating more Pods, not creating more containers inside
    of a single Pod. The Pod is referred to as 'the atom' of Kubernetes

    There are several general use command line commands when it comes to pods including:

    * `kubectl get pods` to return a list of the created Pods and their states (RUNNING, etc.)
    * `kubectl get pods -o wide` similar to the command above but with more information including the Pod's node and internal IP address
    * `kubectl describe pod name` to get a detailed description of the Pod named name

    

=== "ReplicaSets"
    

=== "Deployments"

