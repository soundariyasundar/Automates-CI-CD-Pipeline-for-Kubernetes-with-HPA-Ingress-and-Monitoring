# Automates-CI-CD-Pipeline-for-Kubernetes-with-HPA-Ingress-and-Monitoring
--> Pulling a Docker image from Docker Hub 
--> Deploying it on Kubernetes using Deployment, Service, Ingress, and HPA 
--> Setting up Jenkins for CI/CD (automatic deployment) 
--> Installing and configuring Prometheus & Grafana for monitoring

 Prerequisites:
Installation Tools :
--> Docker (for running containers) 
--> Minikube (to run Kubernetes locally) 
--> Kubectl (to interact with Kubernetes) 
--> Helm (for Prometheus & Grafana) 
--> Jenkins (for CI/CD automation)

START MINIKUBE CLUSTER:
$ minikube start --driver=docker

PULL DOCKER IMAGE:
$ docker pull learnitguide/busapp

DEPLOY APPLICATION ON KUBERNETES
1.Create Deployment 
2.Create Service 
3.Create Ingress

ACCESS APP:
kubectl port-forward svc/grafana 3000:80

 Key Components of Your Project Output
1. CI/CD Pipeline: Jenkins automatically pulls and deploys the latest Docker image.
2. Kubernetes Deployment: Your learnitguide/busapp is deployed and managed in Kubernetes.
3. Ingress Configuration: Your application is accessible externally using a domain like busapp.local.
4. Horizontal Pod Autoscaler (HPA): Ensures automatic scaling of pods based on CPU usage.
5. Monitoring & Logging:
Prometheus: Collects real-time metrics from Kubernetes.
Grafana: Provides a dashboard for visualizing application performance.

How the Final Project Works ?
--> Jenkins triggers CI/CD → Pulls the latest Bus App image and updates the Kubernetes deployment.
--> Application is accessible via Ingress → You can visit http://busapp.local to access it.
--> Autoscaling enabled → Kubernetes automatically scales pods up or down based on traffic and resource utilization.
--> Real-time monitoring with Grafana → Dashboards show CPU, memory usage, pod health, and request rates.

Final View in Grafana:

After logging into Grafana 
"(http://localhost:3000)" you will see a dashboard with real-time metrics for your application, including CPU, memory, and request rates.
The app's performance can be tracked using Prometheus as a data source.

Final Output:
 A complete CI/CD pipeline with Kubernetes, Jenkins, Prometheus, and Grafana.Automatic Kubernetes deployment.Autoscaling enabled with HPA.Real-time monitoring in Grafana.
End Result: A highly available, auto-scalable, and monitored application with a fully automated CI/CD pipeline!
---> Bus App is fully automated & scalable!


![Screenshot (578)](https://github.com/user-attachments/assets/ef108b61-902c-43fc-a27b-16b12db9d18c)


![Screenshot (579)](https://github.com/user-attachments/assets/2428aa86-8bdb-43f9-88fb-5d6931d05f19)


![Screenshot (581)![![Screen![Screenshot (577)](https://github.com/user-attachments/assets/ad6f1d03-0d51-4872-b827-ac86390c3071)
shot (576)](https://github.com/user-attachments/assets/a4949616-6c62-4b62-bd55-61e8d132a587)
Screenshot (575)](https://github.com/user-attachments/assets/8104d158-34cc-4528-b354-1eed06732d6c)
](https://github.com/user-attachments/assets/75357a99-7ee8-45db-88c0-c6140a846df2)
![Screenshot (583)](https://github.com/user-attachments/assets/b5dbae98-cc6b-475c-9b35-1ab41d0c54eb)
![Screenshot (584)](https://github.com/user-attachments/assets/8c8c1735-5298-41b3-a784-5a6d964795ef)
![Screenshot (589)](https://github.com/user-attachments/assets/4a5e52b2-7968-4f67-b448-0621ffb970b3)
