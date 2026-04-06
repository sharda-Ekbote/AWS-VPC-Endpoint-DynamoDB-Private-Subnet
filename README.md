Access AWS DynamoDB from Private Subnet via VPC Endpoint

This project demonstrates how to securely access Amazon DynamoDB from an EC2 instance located in a private subnet without 
using a NAT Gateway or traversing the public internet. This is achieved using a VPC Gateway Endpoint.

Architecture Highlights

VPC: Custom CIDR (10.0.0.0/16).

Subnets: One Public (for Bastion/Jump host) and one Private (for secure workload).

Security: No Internet Gateway or NAT Gateway attached to the private subnet.

Connectivity: AWS PrivateLink (Gateway Endpoint) for DynamoDB.
