# Task
- Deploy multiple instances of a microservice application.
- Create a Kubernetes service to expose the microservices internally.
- Configure an Ingress controller to enable external access to the microservices.
- Implement load balancing among the microservice instances.

# Steps to Achieve

Deploy nginx ingress controller
- `kubectl apply -f ingress-nginx-controller.yaml`

Deploy applications
 - `kubectl apply -f app1.yaml`
 - `kubectl apply -f app2.yaml`

Deploy ingress rules
 - `kubectl apply -f ingress-rules.yaml`

Add entry into /etc/hosts with the local_dns_name and cluster_ip
 - `Test the ingress rules`