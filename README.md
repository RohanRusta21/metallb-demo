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

NOTE : If using manifests , then create ns first. namespace: metallb-system

```bash
kubectl apply -f https://raw.githubusercontent.com/metallb/metallb/v0.14.5/config/manifests/metallb-native.yaml
```

# Installation steps for nginx ingress controller

```bash
helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx
kubectl create namespace nginx-ingress
helm install ingress-nginx ingress-nginx/ingress-nginx -n nginx-ingress
```

# To Check and verify if nginx ingress working or not

```bash
kubectl get svc -n nginx-ingress
```

