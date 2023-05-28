# Mongo Express K8 Cluster Config
This is a simple example of how to deploy a Mongo Express instance to a Kubernetes cluster.

## Execution
To execute this example, run the following commands:

Add secret to cluster

```properties
kubectl apply -f secret.yaml
```
Add MongoDB deployment and internal service to cluster

```properties
kubectl apply -f mongo-config.yaml
```
Add Mongo Express ConfigMap to cluster
```properties
kubectl apply -f mongo-config-map.yaml
```
Add Mongo Express deployment and external service to cluster
```properties
kubectl apply -f mongo-express.yaml
```