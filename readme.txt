kubectl create -f https://download.elastic.co/downloads/eck/2.5.0/crds.yaml
kubectl apply -f https://download.elastic.co/downloads/eck/2.5.0/operator.yaml

kubectl create namespace elastic
kubectl apply -f elasticuser.yaml 

kubectl apply -f deploy.yaml 
kubectl apply -f elk-ingress-prod.yaml 

