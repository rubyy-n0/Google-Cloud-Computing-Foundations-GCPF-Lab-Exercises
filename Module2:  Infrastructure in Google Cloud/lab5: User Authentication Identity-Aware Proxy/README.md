# User Authentication with Identity-Aware Proxy

## Objective
To learn how to deploy a Cloud Run application and secure it using Identity-Aware Proxy (IAP), and understand how user identity information can be accessed and verified securely.

## Key Steps Performed
1. Downloaded and extracted the lab application code.
2. Deployed a simple Cloud Run service using gcloud.
3. Enabled Identity-Aware Proxy (IAP) for the service.
4. Restricted access by granting IAP-secured Web App User role.
5. Tested application access with authenticated Google account.
6. Modified deployment to access user identity headers:
   - X-Goog-Authenticated-User-Email
   - X-Goog-Authenticated-User-ID
7. Verified identity information displayed in application.
8. Disabled IAP to test unprotected access behavior.
9. Observed how identity headers can be spoofed when IAP is disabled.
10. Enabled cryptographic verification using JWT assertion.
11. Added IAP_AUDIENCE environment variable for secure verification.
12. Granted Cloud Run Invoker role to IAP service agent.
13. Verified secure, signed identity data in application.

## Tools / Services Used
- Google Cloud Run
- Identity-Aware Proxy (IAP)
- Cloud Shell
- gcloud CLI
- Python (Flask)
- JWT authentication
- Cloud IAM

## Results
Successfully deployed a Cloud Run web application protected by IAP. Learned how user identity is passed securely, how it can be exposed if IAP is disabled, and how cryptographic verification ensures secure identity validation.
