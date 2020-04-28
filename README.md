

To run crateDb kubernetes cluster use below commands

minikube start --memory 4096

kubectl create namespace crate

kubectl create -f crate-internal-service.yaml --namespace crate

kubectl create -f crate-external-service.yaml --namespace crate

kubectl get service --namespace crate

kubectl create -f crate-controller.yaml --namespace crate

For more info 
https://crate.io/a/run-your-first-cratedb-cluster-on-kubernetes-part-one/
https://crate.io/a/run-your-first-cratedb-cluster-on-kubernetes-part-two/
