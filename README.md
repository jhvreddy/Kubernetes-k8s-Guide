# K8s cheatsheet
How many nodes are part of the cluster
``` 
kubectl get nodes
```
What is the version of k8s running on the nodes
```
kubectl version
```
Flavour and OS on which k8s nodes are running
```
kubectl get nodes -o wide
```
How many pods exist on the system?
```
kubectl get pods
```
Create a new pod with the nginx image, Hint: Use the kubectl run command with the correct image.
```
kubectl run nginx --image=nginx
```
