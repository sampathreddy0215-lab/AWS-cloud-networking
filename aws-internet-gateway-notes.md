# AWS Internet Gateway (IGW)

## What is an Internet Gateway?

An Internet Gateway (IGW) is a horizontally scaled, redundant AWS service that enables communication between a VPC and the Internet.

## Functions

- Provides Internet connectivity for public subnets
- Performs NAT for public IPv4 addresses
- Supports inbound and outbound traffic

## How It Works

1. Attach IGW to a VPC
2. Add a route in the Route Table:
   - Destination: 0.0.0.0/0
   - Target: Internet Gateway
3. Assign a Public IP or Elastic IP to the resource

## Common Use Cases

- Web Servers
- Bastion Hosts
- Public Load Balancers

## Best Practices

- Use IGW only for public-facing resources
- Keep databases in private subnets
- Review route tables regularly
- Combine with Security Groups for access control
