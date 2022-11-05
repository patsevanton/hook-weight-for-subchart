## Install

```
kubectl create namespace loggenerator || true
helm upgrade --install loggenerator -n loggenerator ./loggenerator --wait
kubectl get pod -n loggenerator -w
```

## Remove
```
helm uninstall -n loggenerator loggenerator || true
kubectl delete namespace loggenerator || true
```