# Lab 2: Getting Started with Google Cloud Shell and gcloud

## Overview
 This lab introduced the basic tools used to manage Google Cloud resources through the command line. Using Google Cloud Shell and the gcloud CLI, I learned how to configure a cloud environment, create and manage virtual machines, update firewall rules, and monitor system logs. The lab provided practical experience with cloud resource management without requiring local software installation.

## Objectives

- Understand the purpose and features of Google Cloud Shell.
- Learn how to use the `gcloud` command-line tool.
- Configure default project, region, and zone settings.
- Create and manage a Compute Engine virtual machine (VM).
- Connect to a VM instance using SSH.
- Configure firewall rules to enable web traffic.
- View and filter system and Compute Engine logs.

## Key Activities
Activated Google Cloud Shell and verified project settings.
Configured environment variables for the project ID and compute zone.
Created a virtual machine named gcelab2 using the gcloud compute instances create command.
Explored gcloud help commands and configuration options.
Used filtering commands to display specific Compute Engine instances and firewall rules.
Connected securely to the VM through SSH and installed the Nginx web server.
Added network tags and created a firewall rule to enable HTTP traffic.
Verified web server accessibility using the VM's external IP address.
Examined available system logs and filtered logs related to Compute Engine resources.

## Key Commands Used
gcloud config
gcloud compute instances create
gcloud compute ssh
gcloud compute firewall-rules
gcloud logging logs list
gcloud logging read

## Results
The lab was completed successfully by creating and managing a virtual machine through the gcloud CLI. Firewall rules were configured to allow HTTP traffic, and the Nginx web server was accessed successfully. I also gained experience in viewing and filtering Google Cloud logs for monitoring and troubleshooting purposes.

## Conclusion
This lab provided hands-on experience with the core features of Google Cloud Shell and the gcloud command-line interface. It demonstrated how cloud resources can be configured, managed, and monitored efficiently through terminal commands, building a strong foundation for more advanced Google Cloud administration tasks.
