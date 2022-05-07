### **Minikube**

> *Minikube is a lightweight Kubernetes implementation that creates a VM on your local machine and deploys a simple cluster containing only one node. Minikube is available for Linux, macOS, and Windows systems.*



### **Minikube Installation**

#### **1. To install the latest minikube stable release on x86-64 Linux using binary download:**

```bash
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```

#### **2. Start The Minikube Cluster**

```bash
minikube start
```

#### **3. Install Kubectl commandline tool**

```bash
minikube kubectl -- get po -A
```

#### **4. Add the following line in the $HOME/.bashrc file**

```bash
alias kubectl="minikube kubectl --"
```

#### **5. Test your cluster**

```bash
kubectl get po -A
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