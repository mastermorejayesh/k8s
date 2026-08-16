# 1. Check cluster
kubectl get namespace
kubectl get nodes

# 2. Create namespace
kubectl create namespace nginx

# 3. Create Pod in nginx namespace
kubectl run nginx-pod --image=nginx -n nginx

# 4. Check Pod
kubectl get pods -n nginx

# 5. Delete Pod
kubectl delete pod nginx-pod -n nginx

# 6. Create Deployment from YAML
kubectl apply -f deployment.yml

# 7. Check Deployment
kubectl get deployment

# 8. Check ReplicaSet
kubectl get replicaset

# 9. Check Pods
kubectl get pods

# 10. Enter Pod
kubectl exec -it <pod-name> -- bash

# 11. Change image
kubectl set image deployment/nginx-deployment nginx=nginx:1.16.1

# 12. Watch rollout
kubectl rollout status deployment/nginx-deployment

# 13. Check Pods again
kubectl get pods
