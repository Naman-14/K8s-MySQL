# K8s-MySQL
Deploying MySQL

Accessing our MySQL Instance and showing the created databases in it.

Step 1: Create Kubernetes Secret
kubectl apply -f mysql-secret.yaml

Step 2: Create Persistent Volume and Volume Claim
kubectl apply -f mysql-storage.yaml

Step 3: Create MySQL Deployment
kubectl apply -f mysql-deployment.yaml



![image](https://user-images.githubusercontent.com/78831583/235132657-9e07bbc9-664f-43b6-b68c-c0bd8f5364f0.png)
