```
helm repo add cilium/cilium https://helm.cilium.io
helm repo update
helm template cilium cilium/cilium \
  --version 1.10.5 \
  --namespace kube-system \
  --values values.yaml \
  --output-dir base
```
