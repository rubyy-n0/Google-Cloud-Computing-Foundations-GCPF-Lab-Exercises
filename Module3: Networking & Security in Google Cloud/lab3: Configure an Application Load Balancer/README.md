# Configure an Application Load Balancer with Cloud Armor (GSP215)

## Objective
To deploy a global external Application Load Balancer with backend Managed Instance Groups (MIGs) across multiple regions and secure it using Cloud Armor security policies.

## Key Steps Performed
1. Created firewall rules to allow HTTP traffic (port 80) and health checks.
2. Created instance templates for two regions (Region 1 and Region 2).
3. Deployed Managed Instance Groups (MIGs) in both regions.
4. Verified backend VM instances running in different regions.
5. Created a global external Application Load Balancer.
6. Configured frontend IPv4 and IPv6 endpoints.
7. Created backend service linking both MIGs.
8. Configured health checks for backend validation.
9. Enabled load balancing logging.
10. Tested load balancer using browser access.
11. Created a stress test VM (siege-vm).
12. Installed siege tool and generated traffic load.
13. Observed traffic distribution across regions.
14. Created Cloud Armor security policy (denylist).
15. Blocked siege-vm IP using Cloud Armor rule.
16. Verified 403 Forbidden response from blocked IP.
17. Reviewed Cloud Armor security logs.

## Tools / Services Used
- Google Compute Engine
- Managed Instance Groups (MIG)
- Global External Application Load Balancer
- Cloud Armor Security Policy
- Cloud Logging
- Cloud Shell
- gcloud CLI
- Debian Linux
- siege load testing tool
- Firewall Rules

## Results
Successfully deployed a globally distributed load balancing system with automatic traffic routing across regions. Verified autoscaling and load distribution under stress testing. Implemented Cloud Armor security policy to block malicious traffic and confirmed enforcement via logs.
