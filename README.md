```
kubectl apply -f consul.yml
kubectl apply -f vault.yml
kubectl apply -f lamassu-ca.yml 




Borrar todo y Aplicar todo:

kubectl delete -f lamassu-ca-v4.yml
kubectl delete -f vault.yml
kubectl delete -f consul.yml
kubectl delete -f certs.yml

kubectl delete secret vault-credentials-file
kubectl delete secret lamassu-ca-vault-credentials
kubectl delete secret consul-cert-secret
kubectl delete secret lamassu-ca-cert-secret
kubectl delete secret vault-cert-secret
kubectl delete secret downstream-crt-secret
kubectl delete secret root-ca-secret

kubectl apply -f certs.yml
kubectl apply -f consul.yml
kubectl apply -f vault.yml
kubectl apply -f lamassu-ca-v5.yml
```
