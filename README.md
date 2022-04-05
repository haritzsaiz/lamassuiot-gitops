KUBECTL:

Aplicar los YML:
```
kubectl apply -f certs.yml
kubectl apply -f consul.yml
kubectl apply -f vault.yml
kubectl apply -f secret-job.yml
kubectl apply -f lamassu-ca.yml
kubectl apply -f rabbitmq.yml
kubectl apply -f jaeger.yml
kubectl apply -f lamassu-db.yml
kubectl apply -f auth.yml
kubectl apply -f opa-server.yml
kubectl apply -f ui.yml
kubectl apply -f users-job.yml
```
Borrar los YML: 
```
kubectl delete -f certs.yml
kubectl delete -f consul.yml
kubectl delete -f vault.yml
kubectl delete -f secret-job.yml
kubectl delete -f lamassu-ca.yml
kubectl delete -f rabbitmq.yml
kubectl delete -f jaeger.yml
kubectl delete -f lamassu-db.yml
kubectl delete -f auth.yml
kubectl delete -f opa-server.yml
kubectl delete -f ui.yml
kubectl delete -f users-job.yml
```
Borrar los SECRET:
```
kubectl delete secret auth-cert-secret
kubectl delete secret jaeger-cert-secret
kubectl delete secret lamassu-db-cert-secret
kubectl delete secret rabbitmq-cert-secret
kubectl delete secret lamassu-ca-cert-secret
kubectl delete secret lamassu-ca-vault-credentials
kubectl delete secret vault-credentials-file
kubectl delete secret vault-cert-secret
kubectl delete secret consul-cert-secret
kubectl delete secret downstream-crt-secret
kubectl delete secret root-ca-cert-secret
```
Borrar las carpetas "data" creadas en los nodos
```
sudo rm -r data/
```
