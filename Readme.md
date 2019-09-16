#### https://github.com/dockersamples/example-voting-app

#### https://medium.com/@jinnerbichler/securing-spring-boot-applications-with-keycloak-on-kubernetes-76cdb6b8d674  




https://kubernetes.io/fr/docs/tutorials/hello-minikube/  



node server.js  
docker build -t mytest .  

minikube start  
minikube dashboard  
kubectl create deployment hello-node --image=mytest

Affichez le déploiement  
`kubectl get deployments  `

Voir le Pod  
`kubectl get pods`  

Evenement sur le cluster  
`kubectl get events`  

Voir la configuration de kubectl :  
`kubectl config view`

Exposer le Pod comme un Service Kubernetes
`kubectl expose deployment hello-node --type=LoadBalancer --port=8080`

Nettoyage

Vous pouvez maintenant nettoyer les ressources que vous avez créées dans votre cluster :

`kubectl delete service hello-node`
`kubectl delete deployment hello-node`

Si nécessaire, arrêtez la machine virtuelle Minikube (VM) :

`minikube stop`

Si nécessaire, effacez la VM Minikube :

`minikube delete`