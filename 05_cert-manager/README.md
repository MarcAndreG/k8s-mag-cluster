# Installing and configuring cert manager

```
kubectl create namespace cert-manager
```

```
helm repo add jetstack https://charts.jetstack.io
```

```
helm repo update
```

```
helm upgrade --install cert-manager --namespace cert-manager jetstack/cert-manager
```

```
kubectl -n cert-manager apply -f 05_cert-manager/issuer.yaml
```

Override ingress from step 04 with 05_cert-manager/deployment/ingress-tls.yaml
```
kubectl -n web-app-ingress apply -f 05_cert-manager/deployment/ingress-tls.yaml
```