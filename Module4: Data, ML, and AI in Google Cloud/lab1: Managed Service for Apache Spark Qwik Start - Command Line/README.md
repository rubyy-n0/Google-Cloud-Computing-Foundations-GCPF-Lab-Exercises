# Managed Service for Apache Spark (Dataproc) - Command Line (GSP104)

## Objective
To learn how to create, manage, and scale a Managed Service for Apache Spark cluster using the gcloud command-line tool, and to submit a Spark job for execution.

## Key Steps Performed
1. Configured Dataproc region using gcloud CLI.
2. Enabled and re-enabled the Dataproc API.
3. Configured IAM permissions for Compute Engine service account:
   - Granted Storage Admin role
   - Granted Dataproc Worker role
4. Enabled Private Google Access on default subnet.
5. Created a Dataproc cluster named `example-cluster`:
   - Machine type: e2-standard-4
   - Disk size: 500GB
   - Worker nodes: default configuration
6. Submitted a Spark job to calculate Pi:
   - Used SparkPi example class
   - Executed job on Dataproc cluster
7. Monitored job execution until completion.
8. Updated cluster configuration:
   - Increased worker nodes to 4
   - Reduced worker nodes to 2

## Tools / Services Used
- Google Cloud Dataproc (Managed Apache Spark)
- Cloud Shell
- gcloud CLI
- Apache Spark
- IAM (roles & permissions)
- Compute Engine

## Results
Successfully created a fully managed Apache Spark cluster, executed a Spark job (Pi calculation), and dynamically scaled the cluster by changing the number of worker nodes.
