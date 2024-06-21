# Appliquer les secrets et la configuration pour MongoDB
$ kubectl apply -f mongo-secret.yaml
$ kubectl apply -f mongo-config.yaml

# Déployez ensuite l'application mongo puis appliquez son service
$ kubectl apply -f mongo-deploy.yaml
$ kubectl apply -f mongo-service.yaml

# Enfin, déployez l'application Web puis appliquez son service
$ kubectl apply -f web-deploy.yaml
$ kubectl apply -f web-service.yaml

# Vous voyez les pods pour MongoDB et l'application Web en exécutant :
$ kubectl get pods
