```
HELM:
```

helm install lamassu-k8s . -n lamassu-k8s

helm uninstall lamassu-k8s -n lamassu-k8s

```
To delete the all secrets created
```
kubectl delete secret vault-credentials-file -n lamassu-k8s
kubectl delete secret lamassu-ca-vault-credentials -n lamassu-k8s
kubectl delete secret lamassu-ca-cert-secret -n lamassu-k8s
kubectl delete secret vault-cert-secret -n lamassu-k8s
kubectl delete secret consul-cert-secret -n lamassu-k8s -n lamassu-k8s
kubectl delete secret downstream-crt-secret -n lamassu-k8s
kubectl delete secret root-ca-secret -n lamassu-k8s

```
To delete the created in the folder
```
sudo rm -r ../../../../../data/
```

