### **Minikube**

> *Minikube is a lightweight Kubernetes implementation that creates a VM on your local machine and deploys a simple cluster containing only one node. Minikube is available for Linux, macOS, and Windows systems.*



### **Minikube Installation**

####  **Install the latest minikube stable release on x86-64 Linux using binary download:**

```bash
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```

#### **Start The Minikube Cluster**

```bash
minikube start
```

#### Install Kubectl commandline tool**

```bash
sudo snap install kubectl --classic
```


#### **Test your cluster**

```bash
#Node info
kubectl get nodes -o wide

#Pods running
kubectl get pods -A

```

### **Stop The Minikube Cluster**

```bash
minikube stop
```

### **Delete Cluster**

```bash
minikube delete --all
```

#### *For more details and commands, click [here](https://minikube.sigs.k8s.io/docs/start/)*

#### *Install and set up kubectl on linux, click [here](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)*
