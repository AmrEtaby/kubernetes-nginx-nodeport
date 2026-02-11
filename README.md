# kubernetes-nginx-nodeport
Deploying NGINX on Kubernetes using NodePort
# Kubernetes NGINX Deployment (NodePort)

This project demonstrates how to deploy an NGINX application on Kubernetes
and expose it externally using a NodePort service.

## Technologies
- Kubernetes (MicroK8s)
- Ubuntu
- NGINX

## Steps
1. Deploy NGINX using a Kubernetes Deployment
2. Expose the application using NodePort
3. Access the application from a browser

## Run
```bash
kubectl apply -f nginx-deployment.yaml
kubectl expose deployment nginx-deployment --type=NodePort --port=80
kubectl get svc
