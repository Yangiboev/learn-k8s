# Pod

A Pod is a way to represent a running process in a cluster.


NOTE: 
Hands on
```shell
kubectl run db --image mongo:3.3
```

```shell
kubectl get pods
```

```shell
kubectl delete pod db
```

Declerative syntax of mongo pod
Note:
```shell
kubectl create -f db.yml
```

```shell
kubectl get pods
```

```shell
kubectl get pods -o wide
```

```shell
kubectl get pods -o json
```

```shell
kubectl get pods -o yaml
```

```shell
kubectl describe pod db
```

Debugging the running pod
```shell
kubectl describe -f db.yml
```
```shell
kubectl exec db -- ps aux
```
```shell
kubectl exec -it db -- sh
```
```shell
echo 'db.stats()' | mongo localhost:27017/test
```
```shell
exit
```
```shell
kubectl logs db
```
```shell
kubectl exec db --  pkill mongod
```
```shell
kubectl get pods
```
```shell
kubectl delete -f db.yml
```
```shell
kubectl get pods
```
```shell
kubectl get pods
```
