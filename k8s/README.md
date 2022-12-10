Kubernetes-Microservice-WebApp-MySQL


- Microservice Architecture for Phonebook Web Application (Python Flask) with MySQL using Kubernetes.
- Phonebook Microservice Web Application aims to create a web application with MySQL Database using Docker and Kubernetes to give DevOps the understanding of Microservice architecture.
- In this application, we have a frontend service and a backend service to interact with database service. 
- Each service will be managed by a Kubernetes deployment.
- The backend service will be a gateway for the application and it will serve the necessary web pages for create, delete and update operations while the frontend service will serve a search page in order to conduct read operations. To preserve the data in the database, persistent volume and persistent volume claim concepts should be adopted.

As a cloud engineer, you're requested to deploy the app on an AWS EC2 Instance using Docker and Kubernetes to showcase your project. In order to achieve this goal, you need to;
  - Pull the application code from GitHub repo of your team.
  - Create two docker images for create/update/delete and search pages using `Dockerfile`s.
  - Deploy the app using `Kubernetes`. To do so;
  - Create a database service using MySQL.
  - Use a custom network for the services.
Requested files

ADD/DELETE/UPDATE DEPLOYMENT AND SERVICE
2. web_server_deployment.yml      # To be delivered by DevOps Eng.
3. web_server_svc.yaml        # To be delivered by DevOps Eng.

SEARCH DEPLOYMENT AND SERVICE
2. result_server_deployment.yml   # To be delivered by DevOps Eng.
3. result_server_service.yaml     # To be delivered by DevOps Eng.

DATABASE DEPLOYMENT AND SERVICE
1. mysql_deployement.yml          # To be delivered by DevOps Eng.
2. mysql_service.yaml             # To be delivered by DevOps Eng.
3. persistent_volume.yaml         # To be delivered by DevOps Eng.
4. persistent_volume_claim.yaml   # To be delivered by DevOps Eng.

SECRETS AND CONFIGMAP
1. mysql-secret.yaml              # To be delivered by DevOps Eng.
2. database_configmap.yaml        # To be delivered by DevOps Eng.
3. servers_configmap.yaml         # To be delivered by DevOps Eng.



