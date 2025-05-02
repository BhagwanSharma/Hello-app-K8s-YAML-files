To install the latest minikube stable release on x86-64 Windows using Windows PowerShell
-	New-Item -Path 'c:\' -Name 'minikube' -ItemType Directory -Force
-	Invoke-WebRequest -OutFile 'c:\minikube\minikube.exe' -Uri 'https://github.com/kubernetes/minikube/releases/latest/download/minikube-windows-amd64.exe' -UseBasicParsing
Since there is no virtual machine manager in local desktop, Docker desktop need to install and run in local drive to Start cluster as a virtual Container to execute minikube Kubernetes Environment - From a terminal with administrator access (but not logged in as root), run:
minikube start --driver=docker
Deploying the Hello App to Your Cluster - Once Kubernetes cluster is running, we can deploy the Google hello-app sample-- Create a deployment and expose it on port 8080:
we should see the hello-app deployment and a running pod. If the pod status shows "Running," Hello app application has been successfully deployed to the cluster.
Once we will receive a response like "Hello, world!" on url "127.0.0.1:65111" confirming that our application is running correctly.
Create a directory for minikube Kubernetes YAML files and Export our deployed resources as YAML files
Initialized Git repository and pushed to in this GitHub path/location in public folder repository.
Both Deployment.yaml and service.yaml files are available in this github repository. 
