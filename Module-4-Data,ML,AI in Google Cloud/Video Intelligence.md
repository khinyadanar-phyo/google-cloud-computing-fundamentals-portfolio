# Cloud Video Intelligence API

## Introduction
This lab focuses on using Google Cloud’s **Video Intelligence API** to analyze video content and extract meaningful metadata. The API helps make videos searchable by identifying objects, labels, and events occurring within video frames over time.

In this lab, a sample video stored in Cloud Storage is analyzed to detect labels and generate structured annotations.

## Objectives
- Set up a service account for authentication
- Generate and configure service account key
- Obtain an access token for API requests
- Send a video annotation request using the Video Intelligence API
- Monitor asynchronous operation status
- Retrieve video labeling results

## Key Steps Performed

### 1. Service Account Setup
- Created a service account named `quickstart`
- Generated a service account key file (`key.json`)
- Activated service account authentication using the key file
- Generated an access token for API authorization

### 2. Request Preparation
- Created a JSON request file specifying:
  - Input video stored in Cloud Storage (`gs://spls/gsp154/video/train.mp4`)
  - Feature type: LABEL_DETECTION (to identify objects and entities in video)

### 3. API Request Execution
- Sent a video annotation request to the Video Intelligence API
- The API returned an operation name for asynchronous processing
- Stored operation details for later retrieval

### 4. Operation Monitoring
- Queried the operation status using the operation ID
- Initially received processing metadata including progress tracking
- After completion, received final annotation results

### 5. Result Analysis
The API returned structured video annotations including:
- Detected labels (objects/entities in the video)
- Time segments where each label appears
- Confidence scores for each detection
- Input video reference and metadata

## Results
The Video Intelligence API successfully analyzed the video and extracted meaningful labels such as objects and events appearing in different time segments.

Key outputs included:
- Label annotations for detected entities
- Start and end timestamps for each detection
- Confidence scores indicating detection accuracy
- Full video processing status (completed successfully)

## Conclusion
This lab demonstrated how to use the Cloud Video Intelligence API to analyze video content and extract structured metadata. By setting up service account authentication, sending an annotation request, and monitoring the asynchronous operation, raw video data was converted into meaningful, searchable information.

The process highlights how video analytics can be used for content indexing, media search, and intelligent video processing applications.
