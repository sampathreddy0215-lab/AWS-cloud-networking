# Public vs Private Subnets

## Public Subnet
A public subnet has a route to an Internet Gateway (IGW), allowing resources to access the internet directly.

Examples:
- Web Servers
- Load Balancers
- Bastion Hosts

## Private Subnet
A private subnet does not have a direct route to the Internet Gateway.

Examples:
- Application Servers
- Databases
- Internal Services

## Key Differences

| Feature | Public Subnet | Private Subnet |
|----------|----------|----------|
| Internet Access | Yes | No |
| Uses IGW | Yes | No |
| Hosts Public Services | Yes | No |
| Database Placement | No | Yes |

## Best Practice
Use public subnets for internet-facing resources and private subnets for backend systems to improve security.
