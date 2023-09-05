# Kubernetes

​

## 1. What is Kubernetes, and how would you explain it to someone who has never heard of it before?

Kubernetes is an open-source container orchestration platform used to manage and automate the deployment, scaling, and management of containerized applications. It's a system that helps you efficiently run and oversee your applications, ensuring they run reliably and scale easily.

## 2. Can you describe the basic components of a Kubernetes cluster (such as nodes and control plane) and their role?

There are two main components: nodes and the control plane. Nodes are the worker machines that run containers and host applications, while the control plane manages and oversees the cluster. The control plane consists of components like the API server, etcd, controller manager, and scheduler, which collectively control the cluster's behavior and state.

## 3. How does Kubernetes ensure high availability and fault tolerance of applications within a cluster?

​Kubernetes ensures high availability and fault tolerance through features like replication and self-healing. It replicates Pods across multiple nodes, so if one node fails, the workload continues on other nodes. Additionally, Kubernetes detects and replaces failed Pods automatically, maintaining application availability.

## 4. What is a Kubernetes Service, and why is it important for networking and communication between Pods?

​A Kubernetes Service is an abstraction that defines a set of Pods and a policy for accessing them. It is crucial for networking and communication because it provides a stable endpoint for connecting to a group of Pods, even as Pods scale up or down. This abstraction simplifies network routing and load balancing for applications.

## 5. What is a Pod in Kubernetes, and why is it a fundamental building block for containerized applications?

A Pod is the smallest deployable unit in Kubernetes and represents a single instance of a running process. Pods can contain one or more containers that share the same network namespace and storage volume. They are fundamental because they encapsulate an application's components and resources, making it easier to manage, scale, and maintain containerized applications.
