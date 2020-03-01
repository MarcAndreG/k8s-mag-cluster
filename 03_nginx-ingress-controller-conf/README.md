# Install and configure nginx-ingress controller

* https://github.com/helm/charts/tree/master/stable/nginx-ingress

```
kubectl create namespace nginx-ingress
```
```
helm upgrade --install -n nginx-ingress my-controller stable/nginx-ingress -f 03_nginx-ingress-controller-conf/values.yml
```