**HELM:**


Helm install
```
helm install lamassu-k8s . -n lamassu-k8s

```
Helm uninstall
```
helm uninstall lamassu-k8s -n lamassu-k8s
```

Delete all secrets created
```
kubectl delete secret vault-credentials-file -n lamassu-k8s
kubectl delete secret lamassu-ca-vault-credentials -n lamassu-k8s
kubectl delete secret lamassu-ca-cert-secret -n lamassu-k8s
kubectl delete secret vault-cert-secret -n lamassu-k8s
kubectl delete secret consul-cert-secret -n lamassu-k8s -n lamassu-k8s
kubectl delete secret downstream-crt-secret -n lamassu-k8s
kubectl delete secret root-ca-secret -n lamassu-k8s
```

Delete the folder created in the node
```
sudo rm -r ../../../../../data/
```

