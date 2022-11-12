# ReplicaSets
Most applications should be scalable and all must be fault tolerant. Pods do not provide those features, ReplicaSets do.

```shell
kubectl delete -f hello.yml --cascade=orphan
```
```shell
kubectl get rs
```
```shell
kubectl get pods
```
```shell
kubectl create -f hello.yml --save-config
```
```shell
kubectl get pods
```
```shell
kubectl apply -f hello-scaled.yml
```
```shell
kubectl get pods
```
```shell
POD_NAME=$(kubectl get pods -o name \
   | tai```l -1)

```shell
kubectl delete $POD_NAME
```
```shell
kubectl get pods
```
```shell
POD_NAME=$(kubectl get pods -o name \
    | ta```il -1)

```shell
kubectl label $POD_NAME service-
```
```shell
kubectl describe $POD_NAME
```
```shell
kubectl get pods --show-labels
```
```shell
kubectl label $POD_NAME service=hello
```
```shell
kubectl get pods --show-labels
```
```shell
k3d cluster delete mycluster --all
```