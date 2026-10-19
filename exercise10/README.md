# Exercise 10: Multi-node Minikube with multiple apps

3-node cluster (profile devops-multinode). Product Catalog (2 replicas) and
Shopping Cart (3 replicas), each pod on a different node via podAntiAffinity.

Note: shopping_cart_deployment.yaml uses namespace default (the exercise page used a
namespace that does not exist).

![Nodes](nodes.png)
![Pods across nodes](pods.png)
![Service tests](curl.png)
