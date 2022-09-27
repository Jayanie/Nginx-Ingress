# Nginx-Ingress

This repo contains the deployment, services and ingress resources for header based routing.

We can use this to route the requests that contain a specific header value to a different service. 

**Commands**

- minikube start
- minikube addons enable ingress
- kubectl apply -f backend-deployment.yaml
- kubectl apply -f backend-deployment2.yaml
- kubectl apply -f backend-service.yaml
- kubectl apply -f backend-service2.yaml
- kubectl apply -f ingress1.yaml
- kubectl apply -f ingress2.yaml

Curls

- curl http://hello-world.info -H "test:jayanie"
Output: 
{message: "Hello"} 

- curl http://hello-world.info 

Output:
Hello world!

by http://www.tutum.co

We can add a header using requestly extension in Google Chrome. 



