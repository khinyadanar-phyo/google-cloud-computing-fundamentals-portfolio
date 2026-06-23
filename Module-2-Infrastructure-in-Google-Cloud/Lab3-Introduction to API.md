# Working with Google Cloud APIs and Cloud Storage REST API

## Introduction

Application Programming Interfaces (APIs) enable communication between software applications by providing access to data, services, and computing resources. Google Cloud offers a wide range of APIs that allow developers to integrate cloud services into their applications. In this lab, the concepts of API architecture, HTTP methods, RESTful services, JSON data formats, and authentication mechanisms were explored. Practical experience was gained by using the Cloud Storage JSON/REST API to create a storage bucket and upload files through API requests.

## Objectives

* Understand the fundamentals of APIs and their architecture.
* Learn how RESTful APIs use HTTP methods and endpoints.
* Explore API authentication and authorization mechanisms.
* Enable and manage APIs using the Google Cloud API Library.
* Create a Cloud Storage bucket using the Cloud Storage JSON/REST API.
* Upload files to Cloud Storage through REST API requests.
* Gain hands-on experience interacting with Google Cloud services programmatically.

## Key Steps Performed

### 1. Exploring the API Library

Accessed the Google Cloud API Library.
Searched for and enabled the Fitness API.
Reviewed API documentation, quotas, and usage limits.

### 2. Understanding API Fundamentals

Studied API architecture based on the client-server model.
Learned about HTTP methods such as GET, POST, PUT, and DELETE.
Explored the concept of endpoints and RESTful API design.
Reviewed the role of JSON in API communication.

### 3. Creating a JSON Configuration File

Created a `values.json` file in Cloud Shell.
Defined bucket properties including bucket name, location, and storage class.
Prepared the JSON payload required for API requests.

### 4. Authentication and Authorization

Explored different authentication methods including API Keys, OAuth, and Service Accounts.
Generated an OAuth access token using the OAuth 2.0 Playground.
Configured authentication credentials for Cloud Storage API access.

### 5. Creating a Cloud Storage Bucket via REST API

Set environment variables for the OAuth token and project ID.
Sent an HTTP POST request using the `curl` command.
Created a Cloud Storage bucket using the Cloud Storage JSON/REST API.
Verified successful bucket creation in the Cloud Console.

### 6. Uploading a File via REST API

Uploaded an image file to Cloud Shell.
Configured environment variables for the file path and bucket name.
Used a REST API request to upload the image to Cloud Storage.
Confirmed that the file was successfully stored in the bucket.

## Results

The lab was completed successfully by interacting directly with Google Cloud APIs. An API was enabled through the API Library, authentication credentials were generated using OAuth, and a Cloud Storage bucket was created using REST API requests. A file was then uploaded to the bucket through the Cloud Storage JSON/REST API. The lab demonstrated how cloud resources can be managed programmatically without relying solely on the Google Cloud Console.

## Conclusion

This lab provided practical exposure to API concepts and cloud-based API integration. Through the use of REST API requests, JSON payloads, and OAuth authentication, cloud resources were created and managed efficiently. The experience strengthened understanding of API communication, authentication mechanisms, and programmatic interaction with Google Cloud services, which are essential skills for cloud computing and application development.
