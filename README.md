# kube-cluster-istio-0.7.1
Kubernetes cluster +  MetalLB + Istio 0.7.1 + Jaeger + Bookinfo sample app

## Requirements
* Vagrant
* Virtual Box
* Ubuntu
* IP Addresses
  - 172.16.0.40 for kubemaster
  - 172.16.0.41 for kubenode1
  - 172.16.0.41 for kubenode2
  - 172.16.0.130 to 172,16.0.150 for deployments that require LoadBalancer service type.


## Create directory
mkdir -p /data/vm/vagrant/kubernetes/01-cluster-metallb-istio-0.7.1/logs

## Vagrant setup
* Copy Vagranfile to /data/vm/vagrant/kubernetes/01-cluster-metallb-istio-0.7.1/
* vagrant up

## Validate Kubernetes Cluster
* Browse http://172.16.0.131/productpage 
* Refresh pages a three times, pausing 2 seconds between refresh
* Login using user name "jason" and no password
* Refresh pages a three times, pausing 2 seconds between refresh
* Wait 30 seconds
* Visit http://172.16.0.132 and refresh screen every 10 minutes until the Service list box contains values
* Select istio-ingress from the Service list box
* Click Find Traces button.
