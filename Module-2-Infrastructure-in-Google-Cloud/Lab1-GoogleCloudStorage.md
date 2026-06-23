# Google Cloud Storage: Managing Cloud Storage with gcloud CLI

## Introduction

Google Cloud Storage is a scalable object storage service that allows users to store and retrieve data from anywhere in the world. It supports a variety of use cases, including website hosting, data backup, disaster recovery, and content distribution. In this lab, the Google Cloud Command Line Interface (gcloud CLI) was used to create and manage Cloud Storage resources, demonstrating fundamental cloud storage operations such as bucket creation, object management, and access control.

## Objectives

The objectives of this lab were:

1. To create and configure a Google Cloud Storage bucket.
2. To upload and download objects using the gcloud CLI.
3. To organize data using folders and subfolders within a bucket.
4. To view bucket contents and object details.
5. To configure public access permissions for stored objects.
6. To gain hands-on experience managing cloud storage resources through command-line tools.

## Key Steps Performed

### 1. Bucket Creation

Configured the Google Cloud environment and region.
Created a Cloud Storage bucket using the `gcloud storage buckets create` command.
Verified bucket creation through the Google Cloud Console.

### 2. Object Upload

Downloaded an image file (Ada Lovelace portrait) to Cloud Shell.
Uploaded the image to the Cloud Storage bucket using the `gcloud storage cp` command.
Confirmed successful upload within the bucket.

### 3. Object Download

Downloaded the uploaded image from the bucket back to the Cloud Shell environment.
Verified successful retrieval of the object.

### 4. Folder Management

Created a logical folder structure inside the bucket.
Copied the uploaded image into a folder named `image-folder`.

### 5. Bucket and Object Inspection

* Listed bucket contents using the `gcloud storage ls` command.
* Retrieved detailed information about stored objects, including file size and creation date.

### 6. Public Access Configuration

* Updated object permissions using Access Control Lists (ACLs).
* Granted read access to all users.
* Generated a public URL to make the image accessible via a web browser.

## Results

The lab was completed successfully. A Cloud Storage bucket was created and managed entirely through the gcloud CLI. An image file was uploaded, downloaded, copied into a folder, and its metadata was inspected. Public read access was configured, allowing the object to be accessed through a publicly available URL. The lab demonstrated the practical use of Google Cloud Storage for object management, organization, and secure sharing of data in a cloud environment.

## Conclusion

This lab provided practical experience with Google Cloud Storage and the gcloud CLI. Key cloud storage operations such as bucket creation, file management, folder organization, and access control were successfully performed. The knowledge gained from this lab forms a foundation for managing storage resources in Google Cloud environments and supports future work involving cloud-based applications and data management.

