# K8 Hands On

## Requirements

- Minikube
- Docker (or Podman)
- Kubectl

To verify everything works

1. Run `minikube start`
2. Run `kubectl get nodes`

## Commands

Visualizer
`minikube dashboard`

### Pods

Apply/Update
`kubectl apply -f ./hello.yaml`

Delete
`kubectl delete pod hello`

Access
`kubectl exec -it pod/hello -- /bin/bash`

Get Pod Logs
`kubectl logs hello -f`

### Deployment

Scale/Update Replicas
`kubectl scale deployment/deploy --replicas=10`

Get Logs
`kubectl logs -l jobs=say-hello`

### Service

### Ingress

Add
`minikube addons enable ingress`

### Reference

https://github.com/joellord/handson-k8s
