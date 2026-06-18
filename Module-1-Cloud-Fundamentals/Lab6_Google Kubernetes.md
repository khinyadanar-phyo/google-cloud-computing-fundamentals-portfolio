# Lab 6: Google Kubernetes Engine (GKE)

## Overview

This lab introduced Google Kubernetes Engine (GKE), a managed Kubernetes service that simplifies the deployment, management, and scaling of containerized applications. Using Google Cloud, I created a Kubernetes cluster, deployed a containerized application, exposed it to external users through a Kubernetes service, and removed the cluster after completing the deployment. The lab provided practical experience with container orchestration and demonstrated how Kubernetes automates application management in a cloud environment.

## Objectives

By completing this lab, I learned how to configure a default compute region and zone, create and manage a Google Kubernetes Engine cluster, authenticate and interact with the cluster, deploy a containerized application, expose the application through a Kubernetes service, access the application using an external IP address, and delete the cluster after use.

## Key Activities

The lab started by configuring the default compute region and zone for the Kubernetes resources. A Google Kubernetes Engine cluster was then created using the `gcloud` command-line tool, and authentication credentials were obtained to allow interaction with the cluster.

A sample containerized application was deployed to the cluster using Kubernetes deployment commands. The application was exposed to external users by creating a Kubernetes LoadBalancer service, which automatically assigned an external IP address. The deployed application was successfully accessed through a web browser to verify that it was running correctly.

After confirming that the application was functioning as expected, the Kubernetes cluster was deleted to release the allocated cloud resources and complete the lab.

## Key Commands Used

gcloud config set compute/region

gcloud config set compute/zone

gcloud container clusters create

gcloud container clusters get-credentials

kubectl create deployment

kubectl expose deployment

kubectl get service

gcloud container clusters delete

## Results

The lab was completed successfully by creating a Google Kubernetes Engine cluster and deploying a containerized application. The application was exposed through a Kubernetes service and accessed using its external IP address, confirming successful deployment and connectivity. The cluster was then removed after the application had been tested, demonstrating the complete lifecycle of a Kubernetes workload on Google Cloud.

## Conclusion

This lab provided practical experience with Google Kubernetes Engine and the basic concepts of Kubernetes orchestration. It demonstrated how containerized applications can be deployed, managed, and exposed to users using a managed Kubernetes platform. The lab also highlighted the advantages of GKE, including automated cluster management, scalability, load balancing, and simplified deployment of cloud-native applications.
