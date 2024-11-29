Useful commands

> k create deployment learn-kube-deployment --image=ubuntu 

> k create deployment learn-kube-deployment --image=ubuntu -n learn-k8s

> k create deployment learn-kube-deployment-demo --image=ubuntu -n learn-k8s --dry-run

(It will not create actual resources but run command as we run and check which resources will create) 

> k create deployment learn-kube-deployment-demo --image=ubuntu -n learn-k8s --dry-run=client -o yml 
	(-o for get output of command in yaml format)

Pod - 
    uunit of cluster
Service  - 
Internal and external service, helps for communication between Pods
Ingress - 
For creating URLs which can help to access applications from outside.  
Config map -
Config map which helps for storing data, we can access this data inside container at run time, it store data in key value pair,data format and many formate
Secret - 
Secret is used to store highly sensitive data like username password and api keys, api urls. Which can pass to container at run time
Data storage - 
Attaching the valume to the Pod
Deployment
	Contain bundle of Pod and services that make one application 
StatefulSet 
It’s for applications that manage the state inside the cluster

Master nodes have the following things  
API Server 
Scheduler
Controller manager 
	Etcd

Layers of Abstraction
Deployment manages -> Relicaset manages -> Pod manages -> Containers


> minikube start --vm-driver=hyperkit

> minikube service <service_name> for allocate external IP address

> kubectl get services

> kubectl get nodes

> kubectl get pods

> kubectl create deployment nginx-depl --image=nginx

> kubectl get deployment

> kubectl get replicaset

> kubectl edit deployment nginx-depl

> kubectl logs nginx-depl-6686967ccf-prtlk

> kubectl create deployment mongo-depl --image=mongo

> kubectl create deployment mongo-depl --image=mongo

> kubectl describe mongo-depl-887485654-hh7tw

> kubectl describe pod mongo-depl-887485654-hh7tw

> kubectl logs mongo-depl-887485654-hh7tw

> kubectl exec -it mongo-depl-887485654-hh7tw -- bin/bash

> kubectl delete deployment mongo-depl

> kubectl delete deployment nginx-depl

> Kubectl apply -f <yaml file name>

> Kubectl delete -f <yaml file name>

> kubectl get pods -o wide

> K get all

> minikube service <service_name> for allocate external IP address

> sudo vi /etc/hosts —-------------(Change this file, you can bind local IP’s)

> k get pods

> k get ingress

> k api-resources --namespaced=false

> k get namespaces

