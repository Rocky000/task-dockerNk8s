# task-dockerNk8s

## Steps to Deploy the Application to a Kubernetes Cluster

### Build your Docker image
```shell
$ docker build -t your-docker-username/nodejs-app:latest .
```

### Push the Docker image to a registry

```shell
$ docker push your-docker-username/nodejs-app:latest
```
### Apply the updated Kubernetes Deployment YAML file

```shell
$ kubectl apply -f deployment.yaml
```
### Verify the deployment

```shell
$ kubectl get deployments
$ kubectl get pods
```
With these steps, The Node.js application will be deployed to a Kubernetes cluster with resource limits set for each container.
