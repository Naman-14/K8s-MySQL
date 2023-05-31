# K8s-MySQL
Deploying MySQL

Accessing our MySQL Instance and showing the created databases in it.

Step 1: Create Kubernetes Secret:
kubectl apply -f mysql-secret.yaml

Step 2: Create Persistent Volume and Volume Claim:
kubectl apply -f mysql-storage.yaml

Step 3: Create MySQL Deployment:
kubectl apply -f mysql-deployment.yaml

Step 4: Access Your MySQL Instance:
a) List the pods: kubectl get pod
c) Get a shell for the pod by executing the following command: kubectl exec --stdin --tty (MySQL pod name) -- /bin/bash
d) Type the following command to access the MySQL shell: mysql -p
e) When prompted, enter the password you defined in the Kubernetes secret
f) Now, create the database and access it


![image](https://user-images.githubusercontent.com/78831583/235132657-9e07bbc9-664f-43b6-b68c-c0bd8f5364f0.png)
