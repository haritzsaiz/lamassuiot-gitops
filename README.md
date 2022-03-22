**HELM:**


Helm install
```
helm install lamassu . -n lamassu

```
Helm uninstall
```
helm uninstall lamassu -n lamassu
```

Delete all secrets created
```
kubectl delete secret vault-credentials-file -n lamassu
kubectl delete secret lamassu-ca-vault-credentials -n lamassu
kubectl delete secret lamassu-ca-cert-secret -n lamassu
kubectl delete secret vault-cert-secret -n lamassu
kubectl delete secret consul-cert-secret -n lamassu -n lamassu
kubectl delete secret downstream-crt-secret -n lamassu
kubectl delete secret root-ca-secret -n lamassu
```

Delete the folder created in the node
```
sudo rm -r ../../../../../data/
```

