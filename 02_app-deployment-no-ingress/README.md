# Hello world App deployement

* https://kubernetes.io/fr/docs/concepts/workloads/controllers/deployment/#cr%C3%A9ation-dun-d%C3%A9ploiement
* https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/
* https://kubernetes.io/fr/docs/concepts/services-networking/service/

```
kubectl create namespace web-app
```

```
kubectl -n web-app apply -f 03_app-deployment-no-ingress/deployment/
```