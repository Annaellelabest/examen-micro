# Simple NodeJS Webapp

The application uses an environment variable `APPLICATION_INSTANCE`.  
This variable will be used by the application to listen on a specific path (i.e. `/${application_instance}/health`).

## Launch the application:

```bash
export APPLICATION_INSTANCE=example
node src/count-server.js
```
# RUN Docker
docker build -t  node-app .
docker run -p 8080:8080 -e APPLICATION_INSTANCE=exemple node-app

