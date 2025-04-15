# System Requirements & Setup

The microservice runs on Node.js and requires npm to install dependencies. It uses Express.js for backend routing and basic HTML/JavaScript for the frontend interface. To use the service, simply start the Node.js server, access the HTML page in a browser, and perform calculations. The system is lightweight and can be deployed on any server.

1) Download Node.js (LTS version) from https://nodejs.org/ and install it.

2) Open a terminal and navigate to your preferred directory.

3) Initialize a Node.js project through terminal:
   ```sh
   npm init -y
   ```

4) Clone 5.1p from github 
git clone https://github.com/KvsNikhil/sit737-2025-prac5p.git 

5) Create two yaml files
   deployment.yaml & service.yaml
   
6) Getting pods and kubectl services

kubectl get pods
kubectl get services

7) kubectl port-forward command to forward traffic from a local port to the Kubernetes service

   kubectl port-forward svc/calculator-service 3000:80

8) Creating new docker image
   docker build -t <image_name>

9) Run the application
   kubectl get pods
   kubectl get svc calculator-service
   kubectl port-forward svc/calculator-service 8080:80

10) Access `http://localhost:8080` in a browser.
