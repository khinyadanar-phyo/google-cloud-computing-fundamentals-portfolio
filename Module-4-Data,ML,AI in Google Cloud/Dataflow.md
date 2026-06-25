# Dataflow: Streaming Data from Pub/Sub to BigQuery

## Introduction

This lab focuses on building a real-time data processing pipeline using Google Cloud Dataflow. The pipeline utilizes a Google-provided Dataflow template to read streaming JSON data from a Pub/Sub topic and load it into a BigQuery table. The lab demonstrates how Google Cloud services can be integrated to process, store, and analyze streaming data efficiently.

## Objectives

* Create a BigQuery dataset and table for storing streaming data.
* Create a Cloud Storage bucket for Dataflow resources.
* Deploy a Dataflow streaming pipeline using a pre-built template.
* Stream data from Pub/Sub into BigQuery.
* Query and analyze streaming data using BigQuery.

## Key Steps Performed

1. Disabled and re-enabled the Dataflow API to ensure proper service access.
2. Created a BigQuery dataset named **taxirides**.
3. Created a partitioned BigQuery table named **realtime** with the required schema.
4. Created a Cloud Storage bucket for Dataflow staging and temporary files.
5. Deployed the **Pub/Sub to BigQuery** Dataflow template.
6. Configured the pipeline to read taxi ride data from a public Pub/Sub topic.
7. Configured the pipeline to write streaming data into the BigQuery table.
8. Monitored the Dataflow job execution through the Google Cloud Console.
9. Verified data ingestion by querying records stored in BigQuery.

## Results

The streaming pipeline was successfully deployed and processed real-time taxi ride data. Messages published to the Pub/Sub topic were automatically ingested by Dataflow and stored in the BigQuery table. Query results confirmed that streaming records were continuously loaded into BigQuery, enabling near real-time data analysis.

## Conclusion

This lab provided practical experience with Google Cloud Dataflow for real-time data processing. The integration of Pub/Sub, Dataflow, BigQuery, and Cloud Storage demonstrated an effective architecture for handling streaming data workloads. The use of a pre-built Dataflow template simplified pipeline deployment and highlighted the scalability and efficiency of Google Cloud's data processing services.
