# k8s tips

## Clean up evected pods
```
kubectl get pods | grep Evicted | awk '{print $1}' | xargs kubectl delete pod
```

# K8s Structured Logging
https://github.com/kubernetes/enhancements/pull/1367/files#diff-3aa8edd896257b5b538d386cf36727f4
