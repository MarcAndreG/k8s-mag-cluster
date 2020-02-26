# Install and configure nginx-ingress controller

* https://github.com/helm/charts/tree/master/stable/nginx-ingress

```
kubectl create namespace nginx-ingress

helm install -n nginx-ingress my-controller stable/nginx-ingress -f nginx-ingress-controller-conf/values.yml
```