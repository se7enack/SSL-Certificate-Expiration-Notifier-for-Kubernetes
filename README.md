# SSL-Certificate-Expiration-Notifier-for-Kubernetes
## Public SSL Certificate Expiration Slack Notifier for Kubernetes
Never miss an expiring SSL cert!


#### 1. Edit the yaml and add your slack channel url, domains, and alert threshold
#### 2. Apply the yaml to kube. 
```sh
kubectl apply -f ssl-expiration-checker.yaml
```
