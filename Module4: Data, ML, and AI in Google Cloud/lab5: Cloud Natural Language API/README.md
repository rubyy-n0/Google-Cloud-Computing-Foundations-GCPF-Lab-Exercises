# Cloud Natural Language API: Qwik Start (GSP097)

## Objective
To learn how to use the Google Cloud Natural Language API to perform entity analysis on text using a service account and gcloud command-line tools.

## Key Steps Performed
1. Enabled the Cloud Natural Language API in the Google Cloud project.
2. Created a service account named `my-natlang-sa`.
3. Generated a JSON key file for authentication (`key.json`).
4. Set the environment variable `GOOGLE_APPLICATION_CREDENTIALS` to authenticate API requests.
5. Configured the Google Cloud project environment variable.
6. Ran entity analysis using the gcloud command:
   - `gcloud ml language analyze-entities`
7. Analyzed a sample sentence about Michelangelo Caravaggio.
8. Saved API response output to `result.json`.
9. Viewed extracted entities using `cat result.json`.

## Tools / Services Used
- Cloud Natural Language API
- gcloud CLI
- Service Accounts (IAM)
- JSON Key Authentication
- Cloud Shell

## Results
Successfully extracted entities such as people, locations, and events from a text sample using the Cloud Natural Language API. The output included entity names, types, salience scores, and Wikipedia links.
