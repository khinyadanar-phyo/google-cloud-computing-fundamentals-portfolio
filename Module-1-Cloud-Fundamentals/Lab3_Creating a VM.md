## Lab 3: Create a Virtual Machine

## Overview

This lab introduced the fundamentals of Google Compute Engine by creating and managing virtual machine (VM) instances. Using both the Google Cloud Console and the `gcloud` command-line tool, I learned how to deploy virtual machines, configure machine settings, install an NGINX web server, and establish remote connections through SSH. The lab demonstrated different methods of provisioning and managing cloud infrastructure.

## Objectives

By completing this lab, I was able to:

 Understand the basic concepts of Google Compute Engine virtual machines.
 Create a virtual machine using the Google Cloud Console.
 Create and manage a virtual machine using the `gcloud` command-line tool.
 Configure project region and zone settings.
 Connect to virtual machines securely using SSH.
 Install and verify an NGINX web server on a VM instance.
 Access a web server through the VM's external IP address.

## Key Activities

 Configured the default project region and zone for Compute Engine resources.
 Created a virtual machine named `gcelab` using the Google Cloud Console.
 Configured machine specifications, including the Debian operating system and e2-medium machine type.
 Enabled HTTP traffic by configuring the necessary firewall settings.
 Connected to the VM through SSH and updated the operating system.
 Installed and verified the NGINX web server.
 Accessed the default NGINX webpage using the VM's external IP address.
 Created a second virtual machine named `gcelab2` using the `gcloud compute instances create` command.
 Connected to the VM using the `gcloud compute ssh` command.

## Key Commands Used

 gcloud config set compute/region
 gcloud config set compute/zone
 gcloud compute instances create
 gcloud compute ssh
 sudo apt-get update
 sudo apt-get install -y nginx
 ps auwx | grep nginx

## Results

The lab was completed successfully by creating virtual machine instances through both the Google Cloud Console and the `gcloud` CLI. An NGINX web server was installed and verified to be running correctly, and the default web page was successfully accessed through the VM's external IP address. SSH connectivity and basic VM management tasks were also performed successfully.

## Conclusion

This lab provided practical experience in creating and managing virtual machines on Google Compute Engine. It demonstrated both graphical and command-line approaches to deploying cloud infrastructure while introducing essential concepts such as VM configuration, SSH access, firewall settings, and web server deployment.
