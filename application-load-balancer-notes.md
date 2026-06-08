# AWS Application Load Balancer (ALB)

## What is ALB?

Application Load Balancer (ALB) is a Layer 7 load balancer that distributes HTTP and HTTPS traffic across multiple targets.

## Features

- Layer 7 load balancing
- Path-based routing
- Host-based routing
- SSL/TLS termination
- High availability
- Health checks

## Components

### Listener

Receives incoming traffic on:
- HTTP (80)
- HTTPS (443)

### Target Group

Contains backend resources:
- EC2 Instances
- Containers
- Lambda Functions

### Health Checks

Monitors target health and routes traffic only to healthy targets.

## Path-Based Routing

Examples:

- company.com/app1
- company.com/app2

Traffic is routed based on URL path.

## Host-Based Routing

Examples:

- hr.company.com
- sales.company.com

Traffic is routed based on hostname.

## ALB vs NLB

| Feature | ALB | NLB |
|----------|----------|----------|
| Layer | Layer 7 | Layer 4 |
| Protocols | HTTP/HTTPS | TCP/UDP |
| URL Routing | Yes | No |
| Host-Based Routing | Yes | No |
| Static IP | No | Yes |
| Performance | High | Very High |

## Use Cases

- Web Applications
- Microservices
- Container Applications
- API Gateways
- HTTPS Applications

## Advantages

- Intelligent routing
- SSL offloading
- URL-based routing
- Host-based routing

## Limitations

- Only HTTP/HTTPS traffic
- No static IP support
