# chatbot-docker
A machine learning chatbot is implemented in python and hosted on docker .

#### A web implementation of Chatbot using Flask.

### Running the bot image locally   
<li> docker login

<li> docker pull -t praveengottam/chatbot

<li> docker run --rm -p 5000:5000 --name chatbot praveengottam/chatbot

Chat will be live at [http://localhost:5000/](http://localhost:5000/)

# On PKS  (Assuming cluster is already provisioned)

<li> References creating a PKS cluster
https://docs.pivotal.io/runtimes/pks/1-4/create-cluster.html

<li> Installing (PKS/KUBECTL cli)
https://docs.pivotal.io/runtimes/pks/1-4/installing-kubectl-cli.html
https://docs.pivotal.io/runtimes/pks/1-4/installing-pks-cli.html


<li> Creating a deployment on K8
kubectl create -f pks-deployment.yaml

<li> Creating a service on K8
kubectl create -f pks-service.yaml
