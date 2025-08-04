Create a kind cluster using the kind confi.yml file

Create Namespace

$ kubectl create namespace my-app

Creates Deployment defined in deployment.yml.
$ kubectl apply -f deployment.yml 
$ kubectl get deployments -n my-app

Creates a Service (nginx-srv) to expose the Pods created by the above Deployment.

$ kubectl apply -f service.yml 

Lists all Services in the namespace my-app.
Shows details like ClusterIP, Port, and Type.

$ kubectl get svc -n my-app

Displays all resources in the namespace

$ kubectl get all -n my-app

To access services running inside "Kind  cluster" from your host machine

ec2IP:<service-port>








<img width="2880" height="1800" alt="image" src="https://github.com/user-attachments/assets/4becc5e1-f791-40fb-9bef-cfe8e5712806" />
