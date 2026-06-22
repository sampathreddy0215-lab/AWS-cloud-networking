# AWS Elastic IP (EIP)

## What is an Elastic IP?

An Elastic IP (EIP) is a static public IPv4 address provided by AWS that can be associated with EC2 instances and other AWS resources.

## Benefits

- Static public IP address
- Supports failover
- Simplifies DNS management
- Persistent connectivity
- Supports hybrid environments

## Public IP vs Elastic IP

### Public IP

Changes when an EC2 instance is stopped and started.

### Elastic IP

Remains the same until released.

## EIP Allocation Process

1. Allocate Elastic IP
2. Associate with resource
3. Use for inbound and outbound traffic

## EIP Association

Can be associated with:

- EC2 Instances
- NAT Gateways

## EIP Remapping

Elastic IPs can be moved between resources to support failover.

## NAT Gateway Integration

Private Subnet
→ NAT Gateway
→ Elastic IP
→ Internet

## Pricing Considerations

AWS charges for unused Elastic IP addresses.

## Enterprise Use Cases

- Bastion Hosts
- Public Web Servers
- VPN Gateways
- NAT Gateways
- Disaster Recovery

## Best Practices

- Release unused EIPs
- Use DNS for applications
- Use EIPs only when static addressing is required
