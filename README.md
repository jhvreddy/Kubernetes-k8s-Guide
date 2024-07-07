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
What is the image used to create the new pods? You must look at one of the new pods in detail to figure this out,run below command and look under the containers section.
```
kubectl describe pod newpods-<id>
```
Which nodes are these pods placed on? you must look at all the pods in detail to figure this out. Run the command kubectl describe pod newpods-<id> and look at the node field.
Alternatively run below command and check for the node the pod is placed on
```
kubectl get pods -o wide
```
How many containers are part of the pod webapp?
```
kubectl describe pod webapp
```
What images are used in the new webapp pod?


