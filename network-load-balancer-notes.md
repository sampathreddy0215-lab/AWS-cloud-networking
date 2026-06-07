# AWS Network Load Balancer (NLB)

## What is NLB?

AWS Network Load Balancer (NLB) is a Layer 4 load balancer that distributes TCP, UDP, and TLS traffic across multiple targets.

## Features

- High performance
- Low latency
- Supports TCP and UDP
- Static IP addresses
- High availability
- Multi-AZ support

## Components

### Listener

Receives incoming traffic on specific ports.

Example:
- TCP 80
- TCP 443

### Target Group

Contains backend resources:
- EC2 Instances
- IP Addresses
- Lambda Functions

### Health Checks

Monitors target health and routes traffic only to healthy targets.

## NLB vs ALB

| Feature | NLB | ALB |
|----------|----------|----------|
| Layer | Layer 4 | Layer 7 |
| Protocols | TCP/UDP/TLS | HTTP/HTTPS |
| Static IP | Yes | No |
| URL Routing | No | Yes |
| Performance | Very High | High |

## Use Cases

- Gaming Applications
- VoIP Services
- Financial Applications
- Database Traffic
- High Performance Workloads

## Advantages

- Low latency
- Millions of requests per second
- Static IP support
- High availability

## Limitations

- No URL-based routing
- No host-based routing
- Less application awareness compared to ALB
