# Amazon Route 53

## What is Route 53?

Amazon Route 53 is AWS's scalable DNS service used to route users to applications and AWS resources.

## Hosted Zones

### Public Hosted Zone

Accessible from the internet.

### Private Hosted Zone

Accessible only from associated VPCs.

## DNS Record Types

### A Record

Maps a hostname to an IPv4 address.

### AAAA Record

Maps a hostname to an IPv6 address.

### CNAME Record

Maps one hostname to another hostname.

### Alias Record

AWS-specific record that points to AWS resources such as ALB, NLB, CloudFront, and S3.

### MX Record

Used for mail routing.

### TXT Record

Used for SPF, DKIM, and domain verification.

## Routing Policies

### Simple Routing

Single resource routing.

### Weighted Routing

Traffic distribution based on percentages.

### Latency-Based Routing

Routes traffic to the region with the lowest latency.

### Failover Routing

Routes traffic to backup resources during failures.

### Geolocation Routing

Routes traffic based on user location.

## Health Checks

Monitors endpoints using HTTP, HTTPS, or TCP.

## Enterprise Use Cases

- Disaster Recovery
- Multi-Region Applications
- Global Traffic Management
- Blue-Green Deployments
- DNS-Based Failover

## Key Benefits

- Highly Available
- Scalable DNS
- Health Monitoring
- Traffic Optimization
