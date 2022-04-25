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

Delete all secrets created
```
kubectl delete secret auth-cert-secret -n lamassu
kubectl delete secret consul-cert-secret -n lamassu
kubectl delete secret downstream-crt-secret -n lamassu
kubectl delete secret jaeger-cert-secret -n lamassu
kubectl delete secret lamassu-ca-cert-secret -n lamassu
kubectl delete secret lamassu-ca-vault-credentials -n lamassu
kubectl delete secret lamassu-db-cert-secret -n lamassu
kubectl delete secret rabbitmq-cert-secret -n lamassu
kubectl delete secret root-ca-cert-secret -n lamassu
kubectl delete secret ui-cert-secret -n lamassu
kubectl delete secret vault-credentials-file -n lamassu
kubectl delete secret vault-cert-secret -n lamassu
kubectl delete secret lamassu-device-manager-cert-secret -n lamassu
kubectl delete secret lamassu-dms-enroller-cert-secret -n lamassu
kubectl delete secret lamassu-cloud-proxy-cert-secret -n lamassu
kubectl delete secret test -n lamassu
kubectl delete secret test2 -n lamassu
```

Delete the "/data" folder created in the node
```
cd
sudo rm -r ../../data/
```

