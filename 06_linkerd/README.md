# Installing and configuring linkerd service mesh

* https://linkerd.io/2/getting-started/#step-1-install-the-cli

```
linkerd check --pre
```

```
linkerd install | kubectl apply -f -
```

Add linkerd annotations to pods in a deployment
```
annotations:
  linkerd.io/inject: enabled
```
