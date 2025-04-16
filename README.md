# Kubernetes Project

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

### kubectl apply -f my-node-app.yml (use kubectl get deployments and kubectl get pods to check if the pods were created)

### kubectl apply -f service-my-node-app.yml (create a service to map the ports inside the container to your setup)

### minikube service service-my-node-app (expose the webapp to your localhost)

### kubectl describe my-node-app (Displays all the info about the deployment and the changes made)

### minikube dashboard (A dashboard for monitoring of the pods)
 

