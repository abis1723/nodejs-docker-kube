# nodejs-docker-kube
deploy a node js docker file in kubernetes

# buld the docker image
docker build -t abc/exampleapp:v1.0.0

# upload the image to docker hub
docker push abc/exampleapp:v1.0.0

# you need to install minikube your local system to test locally

# deploy the docker image in kubernetes
kubectl apply -f deployment.yml

# to run the app in broweser
minikube ip 
- to get the ip address of the kube
type in browser address bar-
<IP>:30002
  eg: http://192.168.64.4:30002

# to see the minikube dashboard
minikube dashboard
