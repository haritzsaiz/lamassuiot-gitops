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
kubectl delete secret lamassu-ca-vault-credentials
kubectl delete secret vault-credentials-file
kubectl delete secret auth-cert-secret
kubectl delete secret consul-cert-secret
kubectl delete secret jaeger-cert-secret
kubectl delete secret lamassu-db-cert-secret
kubectl delete secret rabbitmq-cert-secret
kubectl delete secret lamassu-ca-cert-secret
kubectl delete secret vault-cert-secret
kubectl delete secret downstream-crt-secret
kubectl delete secret root-ca-cert-secret
```

Delete the folder created in the node
```
sudo rm -r ../../../../../data/
```

