# Cloud Natural Language API

## Introduction
This lab focuses on using Google Cloud’s Cloud Natural Language API to analyze unstructured text and extract meaningful information. Natural Language Processing (NLP) enables computers to understand human language by identifying entities such as people, places, and events.

In this lab, the API is used to perform entity analysis on sample text and return structured insights including entity type, salience, and metadata.

## Objectives
- Create a service account for Natural Language API authentication
- Generate and configure credentials (JSON key file)
- Set environment variables for authentication
- Use gcloud CLI to access Cloud Natural Language API
- Perform entity analysis on sample text
- Understand API response structure (entities, salience, metadata)

## Key Steps Performed

1. Configure Google Cloud project environment variable:
   export GOOGLE_CLOUD_PROJECT=$(gcloud config get-value core/project)

2. Create service account:
   gcloud iam service-accounts create my-natlang-sa --display-name "my natural language service account"

3. Generate service account key:
   gcloud iam service-accounts keys create ~/key.json --iam-account my-natlang-sa@${GOOGLE_CLOUD_PROJECT}.iam.gserviceaccount.com

4. Set authentication environment variable:
   export GOOGLE_APPLICATION_CREDENTIALS="/home/USER/key.json"

5. Perform entity analysis using Cloud Natural Language API:
   gcloud ml language analyze-entities --content="Michelangelo Caravaggio, Italian painter, is known for 'The Calling of Saint Matthew'."

6. Save output to file:
   cat result.json

7. View results:
   result.json contains extracted entities such as:
   - Michelangelo Caravaggio (PERSON)
   - Italian (LOCATION)
   - The Calling of Saint Matthew (EVENT)

## Results
The API successfully extracted structured entities from the text with:
- Entity name and type
- Metadata (Wikipedia links where available)
- Salience score (importance in text)
- Mentions (how the entity appears in the text)

## Conclusion
This lab demonstrated how to use the Cloud Natural Language API for entity analysis. It shows how unstructured text can be converted into structured data using simple command-line tools.
