Appliquer les secrets et la configuration pour MongoDB
sudo kubectl apply -f mongo-secret.yaml
sudo kubectl apply -f mongo-config.yaml

Déployez ensuite l'application mongo puis appliquez son service
sudo kubectl apply -f mongo-deploy.yaml
sudo kubectl apply -f mongo-service.yaml

Enfin, déployez l'application Web puis appliquez son service
sudo kubectl apply -f web-deploy.yaml
sudo kubectl apply -f web-service.yaml

Vous voyez les pods pour MongoDB et l'application Web en exécutant :
sudo kubectl get pods
