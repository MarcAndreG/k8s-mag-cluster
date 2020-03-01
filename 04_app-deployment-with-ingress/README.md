# Hello world App deployement with nginx ingress controller


```
kubectl create namespace web-app-ingress
```

```
kubectl -n web-app-ingress apply -f 04_app-deployment-with-ingress/deployment/
```