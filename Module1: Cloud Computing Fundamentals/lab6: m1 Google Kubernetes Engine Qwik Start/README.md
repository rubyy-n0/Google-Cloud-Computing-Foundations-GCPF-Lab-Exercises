# Google Kubernetes Engine: Qwik Start (GSP100)

## Objective

To learn how to create and manage a Google Kubernetes Engine (GKE) cluster, deploy a containerized application, expose it using a Kubernetes service, and remove resources after use.

## Key Steps Performed

1. Configured the default compute region and zone using gcloud commands.
2. Created a Kubernetes cluster named `lab-cluster`.
3. Generated authentication credentials for the cluster.
4. Connected kubectl to the cluster.
5. Created a deployment named `hello-server`.
6. Used a container image:
   `gcr.io/google-samples/hello-app:1.0`
7. Exposed the deployment using a LoadBalancer service.
8. Verified external accessibility through the generated external IP.
9. Tested application functionality in a browser.
10. Deleted the Kubernetes cluster after completion.

## Tools / Services Used

* Google Kubernetes Engine (GKE)
* Kubernetes
* Cloud Shell
* gcloud CLI
* kubectl
* Compute Engine
* Container image registry
* Load Balancer

## Results

Successfully created a GKE cluster and deployed a containerized application. The application was exposed externally through a Kubernetes LoadBalancer service and accessed successfully through its public IP address.
