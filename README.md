# K8S_ELT_Pipeline
ELT Pipeline using Apache Airflow and PostgreSQL in Kubernetes 
# *Overview*
Project repo to demonstrate ELT Pipeline using Apache Airflow and PostgreSQL in Kubernetes. Kubernetes is powerful container management, source manegement, scalable hence become useful tool for ELT Pipeline to orchestrate Airflow Webserver and PostgreSQL. The ELT Pipeline by extract JSON file and load into PostgreSQL database, create cleansing table in  PostgreSQL, conduct data cleansing the data.  
# *Prerequisites*
To follow along this project there are requirements need to be available on system:
- Docker
  ```bash
  # install docker
  sudo apt install -y docker-ce docker-ce-cli containerd.io

  # check docker running
  docker --version
  ```
- Minikube
  ```bash
  # download minikube
  curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64

  # install minikube
  sudo install minikube-linux-amd64 /usr/local/bin/minikube

  # checking minikube running
  minikube version
  ```
- Helm
  ```bash
  # install helm
  curl https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3 | bash

  # checking helm running
  helm version
  ```
- Kubectl
  ```bash
  # download the Google Cloud public signing key and add the Kubernetes apt repository to your system
  sudo curl -fsSLo /usr/share/keyrings/kubernetes-archive-keyring.gpg https://packages.cloud.google.com/apt/doc/apt-key.gpg
  echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee      /etc/apt/sources.list.d/kubernetes.list

  # install kubectl
  sudo apt-get update
  sudo apt-get install -y kubectl   
  ```
- Vim (optional)
  ```bash
  sudo apt install vim
  ```
# *Project Flow*
1. 
