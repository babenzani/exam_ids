# exam_ids
exam IDS

# requirement software
1. having account docker hub
2. file service account GCP
3. having cluster k8s

# how to build image
docker build -t ids/hello helloworld

# how to tags image and push to repository
docker tag ids/hello arbenzani/helloarben:hello

# how to push image to repository at docker hub
docker push arbenzani/helloarben:hello

# how to Deploy the resource to the cluster
kubectl apply -f deployment.yaml

# how to Deploy the service
kubectl apply -f service.yaml

# how to get the external IP address of the service
kubectl get services

# how to View a deployed app
curl EXTERNAL_IP_ADDRESS or open browser http://EXTERNAL_IP_ADDRESS