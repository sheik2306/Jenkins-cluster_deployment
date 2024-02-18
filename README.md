# Jenkins-cluster_deployment
Deployment files for Kubernetes Jenkins 



1. minikube start

2. minikube dashboard

```
 kubectl apply -f service.yaml
 kubectl apply -f deployment.yaml
 kubectl apply -f pv.yaml
 kubectl apply -f pvc.yaml
```

3. minikube service jenkins

pod path:
 kubectl get pods
 kubectl exec -it <pod-name> -- /bin/bash


jenkins path:
	/var/hostpath-provisioner/default/jenkins-pvc
based on:
  metadata:
  name: jenkins-pvc


