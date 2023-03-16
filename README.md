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
      1. API Server      --> It is the main part of master mode to which end user will connect the requirement from end user will be given to api server.
      2. ETCD            --> This is a one type of database which has key-pair value the data of APS server is stored in this.
      3. Control Manager --> It will make sure that the actual state of cluster matches to the desired state so it will control the number of nodes or pods.
      4. Scheduler       --> It will check that if new pod is present then it will assign to a new node, also create manages and deletes the pod.
  
  3. Worker Node --
       1. Kubelet        --> One of the most important part of worker node which is connected to api server it also creates and manages pods also sends                                    success or failuer reports to master.
       2. kube-proxy     --> Assigns IP to pods it runs on each pod and this means that each part will get unique IP.
       3. Runtime        --> Works with kubelet here we use the c engine because kubernetes will also go with other contenerization tools like container d,                                rocket. It is used for pulling images start and stops container.
       
       
       
       
       
![Intro_K8s_architecture-d4fd537f533d01c98802e9c01f858eca](https://user-images.githubusercontent.com/108976232/225552949-d255c3f7-824a-4233-9446-22519fddbeec.png)




       
       
      
       
       
  
