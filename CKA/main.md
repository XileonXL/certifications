# Certified Kubernetes Administrator (CKA) Study Guide

## 1. Introduction

### Curriculum

Sections of the CKA:
- 25%: Cluster Architecture, Installation and Configuration
- 15%: Workloads and Scheduling
- 20%: Services and Networking
- 10%: Storage
- 30%: Troubleshooting

### Concepts

Main concepts related to K8s cluster are:

<center><img src="images/concept-diagram.png" alt="Concept Diagram" width="500"/></center>

### Instructions and Recommendations

There are a few instructions for CKA examen:
- You have 2h of time to solve the examen.
- You can use and navigate through Kubernetes documentation.
- There are 6 clusters to be used with different namespaces
- Avoid waste of time typing more than needed (for example, use alias k=kubectl).
- Be familiar with `kubectl`, `kubeadm`and `etcdctl`.
- Command `kubectl api-resources` shows the short name version of each k8s resource.
- Delete using `kubectl delete <resource> --force --grace-period=0` to make it faster.
- Use `kubectl explain <JSONPath>`to get all fields of a resource.

## 2. Cluster Architecture, Installation and Configuration

At a high level, this chapter covers the following concepts:
- Understanding RBAC.
- Installation of a cluster with `kubeadm`.
- Upgrading a version of a K8s cluster with `kubeadm`.
- Backing up and restoring *etc* with `etcdtcl`.
- Understanding a highly available Kubernetes cluster.

### Role-Based Access Control

RBAC defines policies for users, groups, and processes by allowing or disallowing access
to manage API resources
