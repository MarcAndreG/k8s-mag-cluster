# Install and configure external-dns

* https://github.com/helm/charts/tree/master/stable/external-dns#parameters

```
kubectl create namespace external-dns
```
```
helm upgrade --install -n external-dns --set cloudflare.email=<CF_EMAIL> --set cloudflare.apiToken=<CF_API_TOKEN> my-release -f 01_external-dns-conf/values.yaml stable/external-dns
```



