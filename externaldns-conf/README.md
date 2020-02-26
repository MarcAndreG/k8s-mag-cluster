# Install and configure external-dns

* https://github.com/helm/charts/tree/master/stable/external-dns#parameters

```
kubectl create namespace external-dns

export cfApiToken=<TOKEN>

helm install -n external-dns --set cfApiToken=$cfApiToken my-release -f externaldns-conf/values.yaml stable/external-dns
```



