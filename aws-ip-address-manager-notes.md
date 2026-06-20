# AWS IP Address Manager (IPAM)

## What is AWS IPAM?

AWS IP Address Manager (IPAM) helps organizations centrally plan, manage, and monitor IP address usage across AWS accounts and Regions.

## Benefits

- Centralized IP management
- Prevents CIDR overlap
- Multi-account visibility
- Multi-region visibility
- Automated IP tracking

## Components

### Scopes

#### Private Scope

Used for RFC1918 private IP addresses.

#### Public Scope

Used for public IP address management.

### Pools

CIDR blocks available for allocation.

Example:

10.0.0.0/8

### Allocations

CIDR assignments to VPCs and resources.

Example:

- VPC-A → 10.1.0.0/16
- VPC-B → 10.2.0.0/16

## AWS Organizations Integration

Provides centralized IP governance across multiple AWS accounts.

## Enterprise Use Cases

- Multi-Account AWS Environments
- Multi-Region Deployments
- Cloud WAN Architectures
- Transit Gateway Networks
- Hybrid Cloud Designs

## Best Practices

- Plan CIDRs centrally
- Use hierarchical pools
- Monitor utilization
- Avoid overlapping address spaces
