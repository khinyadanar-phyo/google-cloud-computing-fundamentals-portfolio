# Managed Service for Apache Spark

## Introduction

This lab focuses on using Google Cloud's Managed Service for Apache Spark to create, manage, and scale Apache Spark clusters efficiently. The service simplifies cluster deployment and management, enabling large-scale data processing without the complexity of manually configuring infrastructure. The lab demonstrates cluster creation, job execution, and cluster scaling through the command line.

## Objectives

* Create a Managed Service for Apache Spark cluster using the command line.
* Configure the required permissions and network settings.
* Run a sample Apache Spark job on the cluster.
* Modify the number of worker nodes in the cluster.
* Understand cluster scalability and resource management in Google Cloud.

## Key Steps Performed

1. Configured the Dataproc region and enabled the required APIs.
2. Assigned Storage Admin and Dataproc Worker roles to the Compute Engine default service account.
3. Enabled Private Google Access for the default subnet.
4. Created a Managed Service for Apache Spark cluster named **example-cluster** using e2-standard-4 virtual machines.
5. Submitted a sample SparkPi job to calculate an approximate value of π (Pi).
6. Monitored job execution and verified successful completion.
7. Scaled the cluster by increasing the number of worker nodes from the default configuration to four workers.
8. Tested cluster flexibility by reducing the number of worker nodes back to two.

## Results

The Managed Service for Apache Spark cluster was successfully deployed and configured. The SparkPi application executed correctly and produced an approximate value of Pi, confirming successful job processing within the cluster. Cluster scaling operations were completed without interruption, demonstrating the ability to dynamically adjust computing resources based on workload requirements.

## Conclusion

This lab provided practical experience with deploying, managing, and scaling Apache Spark clusters in Google Cloud. The activities demonstrated how Managed Service for Apache Spark simplifies big data processing by automating infrastructure management while providing flexibility for workload scaling. The lab also highlighted the efficiency of using command-line tools to manage Spark environments and execute distributed data processing tasks.
