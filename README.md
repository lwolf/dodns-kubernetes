# Kubernetes manifests for DoDNS
[Kubernetes v1.4 or later is required]

## Edit configmap to match your configuration

Available settings:

* domain - Domain you want to update. Required. Ex. [example.com]
* subdomain - default is `*`
* record - Digital Ocean record id
* checker_url - default is `http://ipecho.net/plain`, could be any service that returns plain ip address
* apikey - Your Digital ocean API key


## Deploy configmap and PeriodicJob manifests

```
# kubectl create -f configmap.yml
# kubectl create -f periodicjob.yml
```
