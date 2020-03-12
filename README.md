# Kubernetes phpMyAdmin
 Deploy phpMyAdmin in Kubernetes

## Prerequisites

* Install [MySQL](github.com/hatamiarash7/Kubernetes-MySQL) first
* Install [helm](https://helm.sh) and repo : `helm repo add bitnami https://charts.bitnami.com/bitnami`


## Install

Set host and port in `helm-values.yml` in `db` section **( You should use MySQL's service name for host )**

```
helm install phpmyadmin -f helm-values.yaml stable/phpmyadmin
```

Read more about helm values [here](https://github.com/helm/charts/tree/master/stable/phpmyadmin)

* You should enable `ingress` to access phpMyAdmin from a web browser
