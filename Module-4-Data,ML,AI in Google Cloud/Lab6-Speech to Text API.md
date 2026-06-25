# Speech-to-Text API – Audio Transcription Lab

## Introduction
This lab focuses on using Google Cloud’s Speech-to-Text API to convert audio into text using machine learning. The API enables developers to integrate speech recognition capabilities into applications by sending audio files and receiving accurate text transcriptions.

In this lab, a pre-recorded audio file from Cloud Storage is used to generate a transcript using API requests.

## Objectives
- Create an API key for Speech-to-Text API authentication
- Configure API restrictions for security
- Create a Speech-to-Text API request using JSON
- Send audio data using Cloud Storage URI
- Call the Speech-to-Text API using curl
- Save and analyze the transcription output

## Key Steps Performed

1. Created an API key from Google Cloud Console:
   - Enabled restriction for Cloud Speech-to-Text API
   - Copied API key for authentication

2. Stored API key as environment variable:
   export API_KEY=<YOUR_API_KEY>

3. Created request file:
   touch request.json

4. Edited request file with audio configuration:
   {
     "config": {
         "encoding": "FLAC",
         "languageCode": "en-US"
     },
     "audio": {
         "uri": "gs://cloud-samples-tests/speech/brooklyn.flac"
     }
   }

5. Sent API request using curl:
   curl -s -X POST -H "Content-Type: application/json"

6. Saved response to file: result.json

7. Viewed output transcription:
   cat result.json

## Results
The Speech-to-Text API successfully converted the audio file into text.

Example output:
- Transcript: "how old is the Brooklyn Bridge"
- Confidence score: ~0.93

The response also included metadata such as:
- Language code
- Processing time
- Request ID

## Conclusion
This lab demonstrated how to use the Speech-to-Text API to convert audio files into text using simple API requests. By configuring authentication, preparing a JSON request, and using curl commands, audio data stored in Cloud Storage was successfully transcribed into readable text.

The exercise highlights how speech recognition can be integrated into applications for transcription, voice assistants, and automated text processing.
