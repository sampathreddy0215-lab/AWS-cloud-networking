# AWS Network Firewall

## What is AWS Network Firewall?

AWS Network Firewall is a managed network security service that provides traffic filtering, intrusion prevention, and centralized inspection for Amazon VPCs.

## Benefits

- Centralized security
- Stateful inspection
- Stateless inspection
- Domain filtering
- High availability
- Scalability

## Components

### Firewall

Inspects network traffic.

### Firewall Policy

Defines traffic handling rules.

### Rule Groups

Contain inspection rules.

#### Stateless Rules

Inspect packets individually.

#### Stateful Rules

Inspect entire connections and sessions.

## Traffic Flow

Internet
→ Internet Gateway
→ Firewall Endpoint
→ Application Subnet
→ EC2

## Logging Options

- CloudWatch Logs
- Amazon S3
- Kinesis Data Firehose

## Domain Filtering

Supports filtering using fully qualified domain names (FQDNs).

## Transit Gateway Integration

Provides centralized inspection for multiple VPCs connected through Transit Gateway.

## Enterprise Use Cases

- Hybrid Cloud Security
- East-West Traffic Inspection
- North-South Traffic Inspection
- Compliance Monitoring
- Threat Prevention

## Best Practices

- Use centralized inspection VPCs
- Enable logging
- Use stateful rules where possible
- Monitor firewall metrics regularly
