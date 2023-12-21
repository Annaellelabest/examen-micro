# Simple NodeJS Webapp

The application uses an environment variable `APPLICATION_INSTANCE`.  
This variable will be used by the application to listen on a specific path (i.e. `/${application_instance}/health`).

## Launch the application:

```bash
export APPLICATION_INSTANCE=example
node src/count-server.js
```
# RUN
## deployement 
1) minikube start
2) kubectl apply -f docker-compose.yaml
-> deployment.apps/node-app created

3) kubectl get deployments
6) kubectl config view

# service

1) kubectl apply -f docker-service.yaml
2) minikube service node-app

