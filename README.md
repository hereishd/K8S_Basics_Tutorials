# K8S Basics Tutorials

Kubernetes is a portable, extensible, open source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.<br/>
In this repo, you can find all my documentation on getting starting with Kubernetes.

## Getting started with K8S

First thing you will need to start your journey in Kubernetes is to install the Kubernetes command line tool: ```kubectl```.
Kubectl will allow you to communicate with a Kubernetes cluster's control plane, using the Kubernetes API, hence to run any 
commands against Kubernetes clusters.<br/><br/>
Second thing you will need is a tool to spin up a Kubernetes cluster. A Kubernetes cluster is a set of nodes that run containerized applications. Here, I will make the use of the tool ```Minikube```. Minikube is a lightweight Kubernetes implementation that creates a VM on your local machine and deploys a simple cluster containing only one node. To begin the journey, it is the perfect tool to allow us to practice and understand. Another tool we could of used to easyly spin up a cluster is ```kind```. I chose Minikube but if you rather go with kind, you can find the steps to install it [here](https://kind.sigs.k8s.io/docs/user/quick-start/).<br/><br/>
With these installed, you should be able to start practicing and understanding the fundamentals. 

## Installing kubectl
Depending on your OS, different steps need to be taken. You can find the method [here](https://pwittrock.github.io/docs/tasks/tools/install-kubectl/) or on the [official kubernetes.io install tools page](https://kubernetes.io/docs/tasks/tools/) under the first paragraph: kubectl.<br/>
Since I am using Ubuntu, I installed it using native package management like this
```
$ sudo apt-get update
$ sudo apt-get install -y apt-transport-https ca-certificates curl
$ curl -fsSL https://pkgs.k8s.io/core:/stable:/v1.28/deb/Release.key | sudo gpg --dearmor -o /etc/apt/keyrings/kubernetes-apt-keyring.gpg
$ echo 'deb [signed-by=/etc/apt/keyrings/kubernetes-apt-keyring.gpg] https://pkgs.k8s.io/core:/stable:/v1.28/deb/ /' | sudo tee /etc/apt/sources.list.d/kubernetes.list
$ sudo apt-get update
$ sudo apt-get install -y kubectl
```
You can then ensure it has been installed running
```
$ kubectl version --client
```
## Installing Minikube


## Reference
* [Offical site's Kubernetes overview](https://kubernetes.io/docs/concepts/overview/)