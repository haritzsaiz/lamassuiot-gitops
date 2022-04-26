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
--repo https://gitlab.com/haritz.saiz/lamassu-kubernetes-v2.git \
--path . \
--dest-server https://kubernetes.default.svc \
--dest-namespace lamassu \
--sync-policy automated \
--auto-prune \
--self-heal
```
