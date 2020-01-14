# k8s tips

## Clean up evected pods
```
kubectl get pods | grep Evicted | awk '{print $1}' | xargs kubectl delete pod
```

## K8s Structured Logging
https://github.com/kubernetes/enhancements/pull/1367/files#diff-3aa8edd896257b5b538d386cf36727f4

## kubectl Tips
https://itnext.io/boosting-your-kubectl-productivity-b348f7c25712

## Remove Zombie Namespaces
https://www.ibm.com/support/knowledgecenter/en/SSBS6K_3.1.1/troubleshoot/ns_terminating.html
