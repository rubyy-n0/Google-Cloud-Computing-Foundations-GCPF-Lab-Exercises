# Dataflow: Qwik Start - Templates (GSP192)

## Objective
To learn how to build a streaming data pipeline using Google Cloud Dataflow templates that transfer data from Pub/Sub to BigQuery.

## Key Steps Performed
1. Re-enabled the Dataflow API using gcloud commands.
2. Created a BigQuery dataset named `taxirides`.
3. Created a BigQuery table named `realtime` with schema for ride data.
4. Created a Cloud Storage bucket using the project ID.
5. Deployed a Dataflow pipeline using the Pub/Sub to BigQuery template.
6. Configured pipeline parameters:
   - Input topic: Pub/Sub public taxi rides dataset
   - Output table: BigQuery taxirides.realtime
7. Monitored Dataflow job in the Google Cloud Console.
8. Verified data ingestion into BigQuery.
9. Queried the dataset using SQL in BigQuery editor.

## Tools / Services Used
- Google Cloud Dataflow
- BigQuery
- Pub/Sub
- Cloud Storage (gsutil)
- Cloud Shell
- gcloud CLI

## Results
Successfully created and executed a streaming data pipeline that reads real-time JSON messages from Pub/Sub and writes them into a BigQuery table using a Dataflow template. Verified data output using SQL queries.
