```
HELM:

helm install lamassu-k8s . -n lamassu-k8s

helm uninstall lamassu-k8s -n lamassu-k8s

kubectl delete secret vault-credentials-file -n lamassu-k8s
kubectl delete secret lamassu-ca-vault-credentials -n lamassu-k8s
kubectl delete secret lamassu-ca-cert-secret -n lamassu-k8s
kubectl delete secret vault-cert-secret -n lamassu-k8s
kubectl delete secret consul-cert-secret -n lamassu-k8s -n lamassu-k8s
kubectl delete secret downstream-crt-secret -n lamassu-k8s
kubectl delete secret root-ca-secret -n lamassu-k8s

sudo rm -r ../../../../../data/





KUBECTL:
Borrar todo y Aplicar todo:

kubectl delete -f lamassu-ca-v7.yml
kubectl delete -f secret-job.yml
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

sudo rm -r data

kubectl apply -f certs.yml
kubectl apply -f consul.yml
kubectl apply -f vault.yml
kubectl apply -f secret-job.yml

kubectl apply -f lamassu-ca-v7.yml

```
