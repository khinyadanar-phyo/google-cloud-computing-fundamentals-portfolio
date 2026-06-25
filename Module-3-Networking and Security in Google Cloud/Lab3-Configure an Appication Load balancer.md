# Configure an Application Load Balancer

## Introduction

This lab focuses on configuring a Global External Application Load Balancer in Google Cloud to distribute traffic across multiple backend regions. The lab also demonstrates how Cloud Armor security policies can be used to protect backend resources by filtering and blocking unwanted traffic at the network edge.

## Objectives

* Configure firewall rules for HTTP traffic and health checks.
* Create instance templates and managed instance groups in multiple regions.
* Deploy and configure a Global External Application Load Balancer.
* Test traffic distribution and failover between backend regions.
* Implement Cloud Armor security policies to block unauthorized traffic.
* Monitor load balancing behavior under high traffic conditions.

## Key Steps Performed

1. Created firewall rules to allow HTTP traffic and health check requests.
2. Configured instance templates with startup scripts and network tags.
3. Created managed instance groups in two different regions with autoscaling enabled.
4. Verified web server deployment and backend accessibility.
5. Configured a Global External Application Load Balancer with IPv4 and IPv6 frontend configurations.
6. Added regional managed instance groups as backend services.
7. Created and configured health checks for backend monitoring.
8. Tested load balancer functionality and verified traffic routing to backend instances.
9. Generated high traffic using a stress-testing virtual machine to observe load distribution behavior.
10. Created a Cloud Armor security policy and denylist rule.
11. Applied the security policy to the backend service and verified that blocked traffic received a 403 Forbidden response.

## Results

The Application Load Balancer was successfully configured to distribute traffic between backend instance groups located in different regions. Health checks ensured that only healthy instances received requests. During stress testing, traffic initially flowed to the nearest backend and was later distributed across multiple regions as demand increased. Cloud Armor successfully blocked traffic originating from the denylisted IP address, preventing unauthorized access to backend resources.

## Conclusion

This lab provided practical experience in deploying and managing a global Application Load Balancer in Google Cloud. It demonstrated how load balancing improves application availability, scalability, and performance across regions. The implementation of Cloud Armor security policies further highlighted the importance of edge-level security in protecting cloud-based applications from unwanted or malicious traffic.
