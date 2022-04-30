Namespace: lamassu

**HELM:**


Helm install
```
helm install lamassu . -n lamassu

```
Helm uninstall
```
helm uninstall lamassu -n lamassu
```

# ArgoCD

```
argocd app create lamassu-gitops \
--repo https://github.com/haritzsaiz/lamassuiot-gitops.git \
--path . \
--dest-server https://kubernetes.default.svc \
--dest-namespace gitops-lamassu \
--sync-policy automated \
--auto-prune \
--self-heal
```

# Kiali, Grafana, Tracing

```

```