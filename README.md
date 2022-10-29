# Kubernetes-Deployment-Service-Example

### Foi utilizado o cluster K8s com minikube

## Comando de criação dos objetos no K8s:

Cria obj deployment: 
kubectl create -f api-deployment --save-config --record

Cria obj service referenciando o deployment:
kubectl create -f api-svc --save-config --record

## Mostra o ip do cluster do K8s+NodePort 
minikube service api-svc --url 

Exemplo:
http://127.0.0.1:53075

Endpoint:
/api/v1/somar?n1=20&n2=30

Completo:
http://127.0.0.1:53075/api/v1/somar?n1=20&n2=30
