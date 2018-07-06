# kube-cluster-istio-0.7.1
Kubernetes cluster +  MetalLB + Istio 0.7.1 + Jaeger

## Create directory
mkdir -p /data/vm/vagrant/kubernetes/01-cluster-metallb-istio-0.7.1/logs

##Vagrant setup
* Copy Vagranfile to /data/vm/vagrant/kubernetes/01-cluster-metallb-istio-0.7.1/
* vagrant up

##Validate Kubernetes Cluster
* Browse http://172.16.0.132 
* Refresh pages a three times, pausing 2 seconds between refresh
* Login using user name "jason" and no password
* Refresh pages a three times, pausing 2 seconds between refresh
* Wait 30 seconds
* Visit http://172.16.0.132 and refresh screen every 10 minutes until the Service list box contains values
* Select istio-ingress from the Service list box
* Click Find Traces button.
