# How to run
## Requirements
- A k8s cluster. This example was tested with [minikube](https://duckduckgo.com)
- [Skaffold](https://skaffold.dev/)
- [Docker](https://www.docker.com/)

## Running
1. Start Docker engine
2. Start Minikube
> minikube start
3. Use skaffold to run project
> skaffold --dev


## Testing
Execute port-forward of order service
> kubectl port-forward service/order 50051:50051

Using `order.proto`
https://github.com/huseyinbabal/microservices-proto/blob/main/order/order.proto to test the grpc call