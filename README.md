# SSL-Certificate-Expiration-Notifier-for-Kubernetes
## Public SSL Certificate Expiration Slack Notifier for Kubernetes
Never miss an expiring SSL cert! 

Creates a kube cronjob that goes out to the internet (daily) to check each of your SSL certs expiration dates. When one or more come within the day threshold set, an alert will be sent to Slack with that information reminding you of the pending expiration.

#### 1. Edit the yaml and add your slack channel incoming webhook url, domains, and alert threshold
#### 2. Apply the yaml to kube. 
```sh
kubectl apply -f ssl-expiration-checker.yaml
```

Slack Notification Example:
<br>
<img src="https://raw.githubusercontent.com/se7enack/SSL-Certificate-Expiration-Notifier-for-Kubernetes/main/example.png"  width="50%" height="50%">

