# Multiple VPC Networks (GSP211)

## Objective
To understand how Virtual Private Cloud (VPC) networks work in Google Cloud by creating custom VPC networks, configuring firewall rules, deploying VM instances, and testing connectivity between isolated networks.

## Key Steps Performed
1. Created custom VPC network: managementnet.
2. Created subnet: managementsubnet-1 (10.130.0.0/20).
3. Created custom VPC network: privatenet.
4. Created subnets:
   - privatesubnet-1 (172.16.0.0/24)
   - privatesubnet-2 (172.20.0.0/20)
5. Configured firewall rules to allow ICMP, SSH, and RDP traffic.
6. Created VM instances:
   - managementnet-vm-1
   - privatenet-vm-1
   - vm-appliance (multi-network interface VM)
7. Tested external connectivity using ping (external IPs).
8. Tested internal connectivity between VPC networks.
9. Verified network isolation between different VPCs.
10. Created VM with multiple network interfaces across 3 networks.
11. Verified routing tables using `ip route`.

## Tools / Services Used
- Google VPC Network
- Compute Engine
- Cloud Shell
- gcloud CLI
- Firewall Rules
- Linux networking tools (ping, ifconfig, ip route)

## Results
Successfully created multiple VPC networks and confirmed that:
- External IPs are reachable across networks
- Internal IPs are isolated between different VPCs
- VM with multiple NICs can communicate across connected subnets
- Routing depends on primary network interface
