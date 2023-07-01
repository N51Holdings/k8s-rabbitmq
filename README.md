# Connect to Kubernetes Cluster

``` gcloud container clusters get-credentials gamepay-staging-cluster --region asia-southeast1 --project powerful-gizmo-360005 ```

## Create a RabbitMQ cluster

```
kubectl create namespace rabbitmq
```

## Install RabbitMQ in GKE

### Create a PVC 
``` 
kubectl apply -f pvc.yaml
```

### Apply Deployent 
``` 
kubectl apply -f deployment.yaml
```

### Apply Service 
``` 
kubectl apply -f service.yaml
```
