In this project, I deployed a simple MongoDB application with the following components:

mongo-config.yaml: This file represents the deployment configuration for the MongoDB database.
web-app.yaml: This file builds on the mongo-express image available on Docker, providing a UI to access the MongoDB database.
secrets.yaml: This file contains secrets related to the MongoDB database.
mongo-config.yaml: This file includes the URL and configuration settings for the MongoDB database.


Prerequiste to run the project-

1) Install docker deskstop
2) Install minikube to run kubernates locally
3) run below commands
   - kubectl apply -f secrets.yaml
   - kubectl apply -f mongo-config.yaml
   - kubectl apply -f mongo-config.yaml
   - kubectl apply -f web-app.yaml
   - minikube service webapp-service (using this command we can directly access UI )
