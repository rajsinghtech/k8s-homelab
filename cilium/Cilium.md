Helm
``` bash
helm install cilium cilium/cilium --version 1.14.3 \
    --namespace kube-system \
    --set kubeProxyReplacement=true \
    --set k8sServiceHost=127.0.0.1 \
    --set k8sServicePort=6443 \
    --set hubble.relay.enabled=true \
    --set hubble.ui.enabled=true \
    --set gatewayAPI.enabled=true
```

[Gateway API](https://docs.cilium.io/en/stable/network/servicemesh/gateway-api/gateway-api/#gs-gateway-api)
