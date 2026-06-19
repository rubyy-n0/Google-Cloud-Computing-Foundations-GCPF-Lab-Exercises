# Cloud IAM: Qwik Start 

## Objective

To understand how Google Cloud IAM manages permissions by assigning, modifying, and removing roles for different users, and to observe how access changes affect Cloud Storage resources.

## Key Steps Performed

Signed in to Google Cloud Console using two accounts (Owner and Viewer).
Explored IAM roles in Cloud IAM and reviewed basic roles (Owner, Editor, Viewer).
Created a Cloud Storage bucket in Cloud Storage using the Owner account.
Uploaded and renamed a sample file inside the bucket.
Verified that the Viewer account could access and view the bucket contents.
Removed the Viewer role from Username 2 in IAM settings and observed loss of access.
Re-assigned access by granting “Storage Object Viewer” role to Username 2.
Used gcloud CLI in Cloud Shell to verify object-level access to the bucket.

## Tools / Services Used

Google Cloud
Google Cloud Console
Cloud IAM
Cloud Storage
Cloud Shell
gcloud CLI

## Results

Successfully demonstrated how IAM roles control access at both project and resource levels. Learned that Owner has full control, Viewer has read-only access, and specific roles like Storage Object Viewer provide limited access to storage resources. Also observed that permission changes take effect after a short propagation delay.
