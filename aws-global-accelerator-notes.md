# AWS Global Accelerator

## What is AWS Global Accelerator?

AWS Global Accelerator improves application performance and availability by routing user traffic through the AWS global network.

## Benefits

- Lower latency
- Improved availability
- Automatic failover
- Global application access
- Static Anycast IP addresses

## Components

### Accelerator

Provides two static Anycast IP addresses.

### Listener

Accepts TCP or UDP traffic.

### Endpoint Group

Represents an AWS Region.

### Endpoint

Resources that receive traffic:

- Application Load Balancer (ALB)
- Network Load Balancer (NLB)
- EC2 Instances
- Elastic IP Addresses

## Traffic Flow

User
→ AWS Edge Location
→ AWS Global Network
→ Endpoint Group
→ Application

## Failover

Traffic automatically shifts to healthy regions during failures.

## Global Accelerator vs Route 53

| Feature | Route 53 | Global Accelerator |
|----------|-----------|-----------|
| DNS Service | Yes | No |
| Static IPs | No | Yes |
| AWS Backbone Usage | No | Yes |
| Traffic Acceleration | Limited | Yes |

## Enterprise Use Cases

- Multi-Region Applications
- Disaster Recovery
- Global Web Applications
- Low-Latency Services
- High Availability Architectures

## Key Benefits

- Faster global access
- Improved reliability
- Seamless failover
- Better user experience
