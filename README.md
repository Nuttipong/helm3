## Deply demo application with Helm3

## Backend
Required
- Pod
- Service
- Secret
```
kubectl create -f backend-secret.yaml
kubectl create -f backend-service.yaml
kubectl create -f backend.yaml
```
## Frontend
Required
- Pod
- Service
- Ingress
```
kubectl create -f frontend-configmap.yaml
kubectl create -f frontend-service.yaml
kubectl create -f frontend.yaml
kubectl create -f ingress.yaml
```
## Mongo
Required
- Pod
- Service
- Secret
- PV
- PVC
```
kubectl create -f mongodb-persistent-volume.yaml
kubectl create -f mongodb-persistent-volume-claim.yaml
kubectl create -f mongodb-secret.yaml
kubectl create -f mongodb-service.yaml
kubectl create -f mongodb.yaml
```

