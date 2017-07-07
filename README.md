# Creating a Kubernetes cluster in google cloud for free

Details of how to use this comments can be viewed viewd here.  

•	Access google cloud console to enable your 300$ free trial https://console.cloud.google.com , and install gloud SDK  https://cloud.google.com/sdk/ 

• Install Kubectl CLI	https://kubernetes.io/docs/tasks/tools/install-kubectl/

•	gcloud components install kubectl

•	gcloud auth login 

•	gcloud container clusters create gke --zone=us-east1-b --scopes “cloud-platform,storage-ro,service-control,service-management,https://www.googleapis.com/auth/ndev.clouddns.readwrite”

•	gcloud config set container/use_client_certificate True

•	export CLOUDSDK_CONTAINER_USE_CLIENT_CERTIFICATE=True


•	gcloud container clusters get-credentials gke --zone us-east1-b --project inner-magpie-170513   Note : that project ID should be tour appropriate project ID

•	kubectl config view

•	kubectl proxy -p 8081 &
