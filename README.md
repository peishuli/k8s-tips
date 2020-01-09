# k8s tips

## Clean up evected pods
```
kubectl get pods | grep Evicted | awk '{print $1}' | xargs kubectl delete pod
```
