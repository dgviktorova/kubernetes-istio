# kubernetes-istio
## Description:
This repo represensts demo for Minikube installation with Helm and Istio MESH.

<img width="603" alt="K8s-istio" src="https://github.com/dianaviktorova/kubernetes-istio/assets/145328524/8598e8f9-d8c7-4e21-b65b-fcafbdb4570f">

## Prerequisites: 
OS - Ubuntu 22.04

## Components of the setup:
- Installing and building local Minikube cluster;
- Installing Helm localy for maing other installations on the cluster;
- Installing and setup Istio MESH from Helm repository;
- Installing testing microservise python app via Helm.
  
## Building the installation:

### Installing and setting up Minikube cluster localy
    Installing Minikube:
    $ curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
    sudo install minikube-linux-amd64 /usr/local/bin/minikube
    $ sudo install minikube-linux-amd64 /usr/local/bin/minikube
    $ minikube start --nodes 1 diana-demo - these steps create one cluster with default namespace
    $ kubectl cluster-info - checking that the cluster is up and running

### Installing Helm localy
    $ sudo apt update
    $ sudo snap install helm --classic
    $ helm version - to check if the CLI tool is installed
    
### Installing Istio MESH
    $ curl -L https://istio.io/downloadIstio | ISTIO_VERSION=1.20.2 TARGET_ARCH=x86_64 sh -
    $ mkdir istio-install
    $ cd Downloads
    $ mv istio-1.20.2-linux-amd64.tar.gz ../istio-install
    $ cd istio-install
    $ tar istio-1.20.2-linux-amd64.tar.gz
    
    In order for istioctl tool to work properly we need to move the PATH to the binary folder of istio installation
    $ 

   
    

