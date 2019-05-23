# chatbot-docker
A machine learning chatbot is implemented in python and hosted on docker .

#### A web implementation of Chatbot using Flask.

### Running locally  
Build the image
docker login

docker pull -t praveengottam/chatbot

Run the image
docker run --rm -p 5000:5000 --name chatbot praveengottam/chatbot

Chat will be live at [http://localhost:5000/](http://localhost:5000/)

# On PKS  (Assuming cluster is already provisioned)

References creating a PKS cluster
https://docs.pivotal.io/runtimes/pks/1-4/create-cluster.html

Installing (PKS/KUBECTL cli)
https://docs.pivotal.io/runtimes/pks/1-4/installing-kubectl-cli.html
https://docs.pivotal.io/runtimes/pks/1-4/installing-pks-cli.html


Creating a deployment on K8
kubectl create -f pks-deployment.yaml

Creating a service on K8
kubectl create -f pks-service.yaml
