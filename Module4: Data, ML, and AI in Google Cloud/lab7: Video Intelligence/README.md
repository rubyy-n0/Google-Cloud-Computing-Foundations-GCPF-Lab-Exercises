# Video Intelligence API: Qwik Start (GSP154)

## Objective
To learn how to use the Google Cloud Video Intelligence API to analyze video content and extract metadata such as labels and objects from video files stored in Cloud Storage.

## Key Steps Performed
1. Enabled and prepared access for the Video Intelligence API.
2. Created a service account for authentication.
3. Generated a service account key file (`key.json`).
4. Activated service account credentials using Cloud Shell.
5. Obtained an access token for API authentication.
6. Created a JSON request file (`request.json`) specifying:
   - Video source (Cloud Storage URI)
   - Feature: LABEL_DETECTION
7. Sent an annotate video request using `curl`.
8. Retrieved an operation ID from the API response.
9. Polled the operation endpoint until processing completed.
10. Received video annotation results including detected labels and timestamps.

## Tools / Services Used
- Google Cloud Video Intelligence API
- Cloud Shell
- Service Account & IAM
- curl command
- JSON request file
- Cloud Storage (video input source)

## Results
Successfully analyzed a video file stored in Cloud Storage and extracted meaningful labels (objects/entities detected in the video). The API returned structured metadata including confidence scores and time segments.
