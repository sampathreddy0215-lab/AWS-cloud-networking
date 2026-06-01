# AWS VPC Peering

## What is VPC Peering?

VPC Peering enables private communication between two VPCs using AWS's internal network.

## Benefits

- Private connectivity
- Low latency communication
- No Internet Gateway required
- Secure traffic flow

## Requirements

- Non-overlapping CIDR ranges
- Route table updates on both VPCs
- Security Group and NACL rules must allow traffic

## Common Use Cases

- Connecting production and development environments
- Cross-account VPC communication
- Multi-region application architectures

## Best Practices

- Plan CIDR ranges carefully
- Update route tables after peering
- Monitor connectivity using VPC Flow Logs
- Use Transit Gateway for large-scale hub-and-spoke designs
