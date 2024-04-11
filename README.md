##Create cluster for test:
```
k3d cluster create mycluster
k3d cluster list
kubectl config get-contexts
kubectl create deployment nginx --image=nginx
kubectl scale deployment nginx --replicas=3
kubectl get pods
kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
kubectl get pods -n kube-system | grep metrics-server
kubectl api-resources --api-group=metrics.k8s.io
kubectl top pods
kubectl top nodes
```

##Start, restart:
```
k3d cluster list
k3d cluster stop mycluster
k3d cluster start mycluster
```

##Delete:
```
k3d cluster list
k3d cluster delete mycluster
```

