# VPC Networks: Controlling Access

## Introduction

This lab focuses on securing web server deployments in Google Cloud using Virtual Private Cloud (VPC) networking. The activities demonstrate how firewall rules, network tags, service accounts, and IAM roles can be used to control access to cloud resources while maintaining security and availability.

## Objectives

* Create Nginx web servers within a VPC network.
* Configure tagged firewall rules to control HTTP access.
* Create and manage service accounts with IAM roles.
* Explore the permissions associated with Network Admin and Security Admin roles.
* Understand the implementation of access control mechanisms in Google Cloud.

## Key Steps Performed

1. Created two virtual machine instances named **blue** and **green** in the default VPC network.
2. Assigned the **web-server** network tag to the blue instance.
3. Installed and configured Nginx on both virtual machines.
4. Customized the default Nginx web pages to distinguish between the two servers.
5. Created a firewall rule allowing HTTP and ICMP traffic only to instances with the **web-server** tag.
6. Deployed a **test-vm** instance to verify network connectivity.
7. Tested internal and external HTTP access to both web servers.
8. Created a service account with the **Compute Network Admin** role.
9. Verified role permissions related to firewall management.
10. Updated the service account with the **Compute Security Admin** role and tested firewall rule administration capabilities.

## Results

Both Nginx web servers were successfully deployed and configured. Internal HTTP communication was accessible between instances within the VPC network. External HTTP access was available only for the blue server due to the applied network tag and firewall rule configuration. Role-based access testing confirmed that the Network Admin role allowed viewing network resources, while the Security Admin role provided permissions to manage firewall rules.

## Conclusion

The lab provided practical experience in implementing network security and access control within Google Cloud. The use of VPC networks, firewall rules, network tags, service accounts, and IAM roles demonstrated how cloud resources can be protected through controlled access and role-based permissions. The activities strengthened understanding of cloud networking and security management concepts.
