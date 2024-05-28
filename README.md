# 🎥 Netflix Clone AKS Deployment Using Services

This repository contains the necessary YAML files to deploy a Netflix Clone application on Azure Kubernetes Service (AKS). The deployment includes a Deployment controller, a Cluster IP service, and a LoadBalancer service.

## 📁 Files

Deployment_NetflixClone.yaml: Contains the YAML configuration for the AKS Deployment controller with the Netflix Clone image.
ClusterIP.yaml: Contains the YAML configuration for the Cluster IP service in Kubernetes.
LoadBalancer.yaml: Contains the YAML configuration for the LoadBalancer service in Kubernetes.

## 🚀 Prerequisites

Before deploying the Netflix Clone application, ensure you have the following:

An active Azure account
An AKS cluster set up
kubectl configured to interact with your AKS cluster

## 🛠️ Deployment Steps

## 1. Clone the repository:

git clone <Link>
cd AKS-Netflix-Clone-SVC

## 2. Deploy the Netflix Clone application:

Apply the Deployment controller configuration:

kubectl apply -f Deployment_NetflixClone.yaml

## 3. Create the Cluster IP service:

Apply the Cluster IP service configuration:

kubectl apply -f ClusterIP.yaml

## 4. Create the LoadBalancer service:

Apply the LoadBalancer service configuration:

kubectl apply -f LoadBalancer.yaml

## 5. Verify the deployment:

Check the status of your pods:

kubectl get pods
Ensure all pods are running successfully.

Check the services:

kubectl get services
Ensure the services are correctly configured and running.

## 🌐 Accessing the Application

Once the LoadBalancer service is created and running, you can access the Netflix Clone application using the external IP provided by the LoadBalancer service. To get the external IP, run:

kubectl get services
Look for the LoadBalancer service and note the EXTERNAL-IP value. Open your web browser and navigate to this IP address to access the Netflix Clone application.

## 📂 Repository Structure


AKS-Netflix-Clone-SVC/
│
├── Deployment_NetflixClone.yaml
├── ClusterIP.yaml
└── LoadBalancer.yaml

## 🤝 Contributing

If you wish to contribute to this repository, please fork the repository and submit a pull request with your proposed changes. Ensure your code adheres to the repository's coding standards and includes appropriate documentation.

## 📧 Contact

For any inquiries or issues, please open an issue on this repository or contact the repository owner at subhojit1@outlook.com.
