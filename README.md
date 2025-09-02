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
- Kubectl
- Vim (optional)
# *Project Flow*
