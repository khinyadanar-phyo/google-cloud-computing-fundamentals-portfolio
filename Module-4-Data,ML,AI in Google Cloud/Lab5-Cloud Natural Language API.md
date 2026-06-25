# Cloud Natural Language API – Entity Analysis Lab

## Introduction

This lab focuses on using Google Cloud’s **Cloud Natural Language API** to analyze unstructured text and extract meaningful information. Natural Language Processing (NLP) enables computers to understand human language by identifying entities, sentiment, and relationships within text.

In this lab, the Cloud Natural Language API is used to perform **entity analysis**, which detects important elements such as people, places, events, and organizations from a given text input.

## Objectives

- Create a service account for API authentication  
- Generate and configure credentials for Cloud Natural Language API  
- Set environment variables for authentication  
- Enable and use the Natural Language API via gcloud CLI  
- Perform entity analysis on sample text  
- Understand API response structure including entities, salience, and metadata  

## Key Steps Performed

### 1. Project and Environment Setup
- Configured Google Cloud project using environment variables
- Created a service account for Natural Language API access
- Generated JSON key file for authentication
- Set `GOOGLE_APPLICATION_CREDENTIALS` environment variable

### 2. API Key and Authentication
- Created service account: `my-natlang-sa`
- Generated service account key file (`key.json`)
- Configured authentication for API access

### 3. Entity Analysis Request
- Connected to Compute Engine VM via SSH
- Used Cloud Natural Language API to analyze text:
