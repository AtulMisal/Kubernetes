# Kubernetes
# This repo has information on kubernetes.

Kubernetes is also knows as k8s because there are 8 characters between k & s.
k8s is an container orchastration an management tool.
   "K8S is an open source system for automating deployment, scalling and managment of containerized application"
    container management (orchestration) tool"

Q) What is mean by Orchestration/Management tool?
  Container orchestration automates the deployment, management, scaling, and networking of containers across the cluster.
  As we know docker is used to create containers but to manage them we use k8s. 
  
Kubernetes is a popular container orchestration tool similar to docker swarm, K8 is mostly used to manage the containers, it is also used for blue-green deployments,    also use to scale the containers.
Written in Golang.

# K8s architecture and overview --
     K8 nodes are divided into 2 types, master node(control plane), and worker node
     These nodes can be a physical machines as well as the virtual machines
     Master and Worker nodes have different components resided inside it
     
  1. Master Node --
     Master is responsible for managing the complete cluster.
     You can access master node via the CLI, GUI, or API.
     The master watches over the nodes in the cluster and is responsible for the actual orchestration of containers on the worker nodes.
     For achieving fault tolerance, there can be more than one master node in the cluster.
     It is the access point from which administrators and other users interact with the cluster to manage the scheduling and deployment of containers.
     It has four components: ETCD, Scheduler, Controller and API Server 
  
  2. Master Node Component --
      1. API Server      -->
      2. ETCD            -->
      3. Control Manager -->
      4. Scheduler       -->
  
  3. Worker Node --
       1. Kubelet        -->
       2. kube-proxy     -->
       3. Runtime        -->
       
       
       
       
       
![Intro_K8s_architecture-d4fd537f533d01c98802e9c01f858eca](https://user-images.githubusercontent.com/108976232/225552949-d255c3f7-824a-4233-9446-22519fddbeec.png)




       
       
      
       
       
  
