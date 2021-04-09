# learnk8

Prereq 

#install Docker
yum install docker
yum install -y yum-utils device-mapper-persistent-data lvm2
systemctl enable docker.service
systemctl start docker

#install Kubectl
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl


#Creating minikube

 curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
 sudo install minikube-linux-amd64 /usr/local/bin/minikube
 
 minikube start --driver=docker
