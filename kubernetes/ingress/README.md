> ### Prerequisites

Enable nginx-ingress controller in minikube

```bash
minikube addons enable ingress
```

> ### *How to deploy the objects*
```bash
1. kubectl apply -f deployment.yaml

2. kubectl apply -f service.yaml

3. kubectl apply -f ingress.yaml
```

> ### *How to delete the objects*

```bash
1. kubectl delete -f ingress.yaml

2. kubectl delete -f service.yaml

3. kubectl delete -f deployment.yaml
```

