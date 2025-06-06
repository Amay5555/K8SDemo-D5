﻿# Kubernetes Project

## Objectives
### Understand Kubernetes by creating a cluster locally using minikube and creating deployment from a YAML config file.
### Check logs and view information about the cluster 

## Tools used
### Kubernetes
### Minikube
### Docker

## Procedure
### Create a YAML config file. Refer to the sample provided on the official site.

### Edit the file and fill in the desired values (deployment name, number of replicas and the image you want to run)

### Create another YAML file to expose the container to access the webpage.

### Start minikube and then run your config file.

### minikube start
<img width="667" alt="minikube start" src="https://github.com/user-attachments/assets/8840aef0-79aa-4fcd-b62a-79c811dfe79b" />

### kubectl apply -f my-node-app.yml (use kubectl get deployments and kubectl get pods to check if the pods were created)

### kubectl apply -f service-my-node-app.yml (create a service to map the ports inside the container to your setup)
<img width="539" alt="applying yml file" src="https://github.com/user-attachments/assets/d97b526a-0d17-41dd-b282-726aafa2eae7" />

### minikube service service-my-node-app (expose the webapp to your localhost)
<img width="552" alt="running the service" src="https://github.com/user-attachments/assets/205c1e85-72ca-4004-9110-8bbaed99fb7b" />
<img width="1279" alt="running site" src="https://github.com/user-attachments/assets/f5fa77b1-af53-4d99-ac03-b2631e72efdf" />

### kubectl get pods (to view all the running pods)
<img width="399" alt="getpods" src="https://github.com/user-attachments/assets/851fafcc-d243-44fc-a548-4bfd8b225e79" />

### kubectl scale deployment my-node-app --replicas=3 (to make sure that 3 pods are ready to run at all times)
<img width="411" alt="scaling" src="https://github.com/user-attachments/assets/92d22703-7d04-4a68-bf4b-fac37ecdff68" />


### kubectl describe my-node-app (Displays all the info about the deployment and the changes made)
<img width="671" alt="describe" src="https://github.com/user-attachments/assets/4eeed5aa-0d91-480e-a63f-0e76b2d56df8" />


### minikube dashboard (A dashboard for monitoring of the pods)
 <img width="1065" alt="minikube dashboard" src="https://github.com/user-attachments/assets/0d6a5498-9fb1-4180-8978-0687fbbbd6ec" />


