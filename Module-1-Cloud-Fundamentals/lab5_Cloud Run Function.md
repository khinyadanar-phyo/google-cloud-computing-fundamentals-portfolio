# Lab 5: Cloud Run Functions Qwik Start – Command Line

## Overview

This lab introduced Google Cloud Run Functions, a serverless computing service that executes code in response to events without requiring developers to manage servers or infrastructure. Using the Google Cloud command line, I created a Cloud Run function, configured its dependencies, deployed it with a Pub/Sub trigger, tested its execution, and monitored its output through Cloud Logging. The lab demonstrated how event-driven applications can automatically respond to cloud events and process data efficiently.

## Objectives

By completing this lab, I learned how to create a Cloud Run function, configure its runtime environment, deploy and test the function using the Google Cloud command line, trigger the function with Pub/Sub messages, and monitor its execution through Cloud Logging.

## Key Activities

The lab began by configuring the default Cloud Run region and creating a project directory for the function code. A Node.js Cloud Run function was developed using the Google Functions Framework and configured to respond to Pub/Sub events. The required dependencies were installed using npm, and the function was prepared for deployment.

The function was then deployed to Google Cloud using the `gcloud functions deploy` command with a Pub/Sub topic as the event trigger. After deployment, the function status was verified to ensure that it was active and ready to receive events.

To test the function, a message was published to the Pub/Sub topic. This triggered the Cloud Run function, which processed the event and generated output in Cloud Logging. Finally, the function logs were viewed using the command line to confirm that the event had been received and processed successfully.

## Key Commands Used

gcloud config set run/region

mkdir

nano index.js

nano package.json

npm install

gcloud functions deploy

gcloud functions describe

gcloud pubsub topics publish

gcloud functions logs read

## Results

The lab was completed successfully by creating and deploying a Cloud Run function through the command line. The function responded correctly to Pub/Sub events, processed the incoming message, and generated the expected output in Cloud Logging. The deployment, testing, and log monitoring processes confirmed that the event-driven application was functioning as intended.

## Conclusion

This lab provided practical experience with Google Cloud Run Functions and serverless computing. It demonstrated how event-driven applications can be developed, deployed, and managed without maintaining server infrastructure. Through the use of Pub/Sub triggers and Cloud Logging, the lab highlighted the simplicity and scalability of serverless architectures for handling automated cloud events and lightweight application workloads.

