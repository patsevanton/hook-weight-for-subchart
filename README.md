## Install

```
kubectl create namespace loggenerator || true
helm upgrade --install loggenerator -n loggenerator ./loggenerator --wait
```

## Remove
```
helm uninstall -n loggenerator loggenerator || true
kubectl delete namespace loggenerator || true
```