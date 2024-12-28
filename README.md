# k8s
<h1>K8S based on kubernetes sample project for learn kubernetes </h1>

<h4> 1. NGINX  </h4>
<h4> 2. Sample Static Website </h4>

1./NGINX

kubectl apply -f deployemnt.yml --------
(it will deploy deployemnt .yml file to deploy application )

kubectl apply -f service.yml-----------
(service.yml file used to access application outsid to world on different services like Cluster-ip,Nodeprt-mode,loadbalancer)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

kubectl get deploy -----to see deployments

kubectl get svc  ----------- to see services
