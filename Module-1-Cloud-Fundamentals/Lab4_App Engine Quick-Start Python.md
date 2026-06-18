# Lab 4: App Engine Qwik Start-Python

## Overview

This lab introduced Google App Engine, a serverless platform that allows developers to deploy and manage applications without handling the underlying infrastructure. Using a Python sample application, I learned how to set up the App Engine environment, test an application locally, modify its code, and deploy it to Google Cloud. The lab demonstrated how App Engine simplifies application hosting by automatically managing scaling, load balancing, and server maintenance.

## Objectives

By completing this lab, I was able to:

Understand the purpose and features of Google App Engine.
Enable the App Engine Admin API.
Download and configure a Python sample application.
Create and activate a Python virtual environment.
Test the application locally using the Flask development server.
Modify the application source code and verify the changes.
Deploy the application to Google App Engine.
Access the deployed application through a web browser.

## Key Activities

Enabled the Google App Engine Admin API.
Cloned the Python sample application repository from GitHub.
Configured a Python virtual environment for the project.
Ran the Flask development server to test the application locally.
Modified the application message from "Hello World!" to "Hello, Cruel World!".
Verified the updated application through the local development server.
Deployed the application to Google App Engine using the `gcloud` command-line tool.
Opened the deployed application in a browser and confirmed successful deployment.

## Key Commands Used
  git clone
  python3 -m venv
  source myenv/bin/activate
  flask --app main run
  nano main.py
  gcloud app deploy
  gcloud app browse

## Results

The lab was completed successfully by deploying a Python web application to Google App Engine. The application was tested locally, updated with custom content, and deployed to the cloud. The deployed application was accessible through its App Engine URL, demonstrating the functionality of a serverless application hosting platform.

## Conclusion

This lab provided practical experience with Google App Engine and serverless application deployment. It demonstrated the complete application lifecycle, including setup, local testing, code modification, and cloud deployment. The lab highlighted how App Engine enables developers to focus on application development while Google Cloud manages the underlying infrastructure and scaling requirements.
