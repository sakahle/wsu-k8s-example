1. Clone example repository: `https://github.com/sakahle/wsu-k8s-example` and switch to that directory `cd wsu-k8s-example`
2. Start minikube `minikube start`
3. Create the deployment `kubectl apply -f example-nginx.yaml`
4. Create a new Service object `kubectl expose deploy nginx-example --type=NodePort --port 80`
5. Get a URL to access your web server: `minikube service nginx-example --url`
6. Copy and paste the output into your browser and check results
