# metallb-demo

# Official Website

```bash
https://metallb.universe.tf/installation/
```

# Installation with Helm 

```bash
helm repo add metallb https://metallb.github.io/metallb
helm install metallb metallb/metallb
```

# Installation with Manifests

```bash
kubectl apply -f https://raw.githubusercontent.com/metallb/metallb/v0.14.5/config/manifests/metallb-native.yaml
```
