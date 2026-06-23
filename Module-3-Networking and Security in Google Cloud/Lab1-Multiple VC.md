# Google Cloud VPC Networking and Multiple Network Interfaces

## Introduction

Google Cloud Virtual Private Cloud (VPC) provides secure and isolated networking environments for cloud resources. VPC networks allow organizations to control network traffic, manage access through firewall rules, and connect resources across different regions. In this lab, multiple custom VPC networks were created, virtual machine instances were deployed, connectivity between networks was tested, and a multi-network VM instance was configured using multiple network interfaces.

## Objectives

* Create custom mode VPC networks and subnets.
* Configure firewall rules for network access control.
* Deploy VM instances in different VPC networks.
* Explore connectivity between VM instances across networks.
* Create and configure a VM with multiple network interfaces.
* Understand network isolation and routing behavior in Google Cloud.

## Key Steps Performed

### 1. Created Custom VPC Networks

* Created a custom VPC network named **managementnet** with a dedicated subnet.
* Created a custom VPC network named **privatenet** with two subnets in different regions.
* Verified the creation of networks and subnets using both the Google Cloud Console and Cloud Shell commands.

### 2. Configured Firewall Rules

* Created firewall rules to allow SSH (TCP 22), RDP (TCP 3389), and ICMP traffic.
* Applied firewall configurations to both **managementnet** and **privatenet**.
* Verified firewall rule deployment and network accessibility settings.

### 3. Deployed Virtual Machine Instances

* Created **managementnet-vm-1** within the managementnet subnet.
* Created **privatenet-vm-1** within the privatenet subnet.
* Verified successful deployment and network assignments of all VM instances.

### 4. Tested Network Connectivity

* Performed connectivity tests using external IP addresses between VM instances.
* Verified successful communication through public network access.
* Tested internal IP communication between instances.
* Observed that VM instances within the same VPC network could communicate internally, while instances in separate VPC networks remained isolated.

### 5. Configured a Multi-Network VM Instance

* Created **vm-appliance** with three network interfaces.
* Connected the VM to:

  * privatenet
  * managementnet
  * mynetwork
* Verified interface configurations and assigned IP addresses.
* Examined routing tables and tested connectivity across connected networks.

## Results

The lab was completed successfully by creating multiple custom VPC networks, configuring firewall rules, and deploying virtual machine instances. Connectivity testing confirmed that communication through internal IP addresses is allowed only within the same VPC network unless additional networking configurations are implemented. A multi-network VM instance was also successfully deployed, demonstrating how a single VM can connect to multiple VPC networks using separate network interfaces.

## Conclusion

This lab provided practical experience in designing and managing Google Cloud VPC environments. It demonstrated network isolation, firewall rule implementation, VM deployment, connectivity testing, and multi-network configurations. These concepts are essential for building secure, scalable, and well-structured cloud networking architectures.
