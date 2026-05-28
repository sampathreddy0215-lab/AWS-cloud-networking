# Security Groups vs Network ACLs (NACLs)

## Definition

### Security Group
A Security Group is a virtual firewall attached to an EC2 instance that controls inbound and outbound traffic.

### Network ACL (NACL)
A Network ACL is a subnet-level firewall that controls inbound and outbound traffic for an entire subnet.

---

# Differences

| Feature | Security Group | NACL |
|---|---|---|
| Applied To | EC2 Instance | Subnet |
| Type | Stateful | Stateless |
| Supports Allow Rules | Yes | Yes |
| Supports Deny Rules | No | Yes |
| Rule Evaluation | All rules evaluated | Rules evaluated in order |
| Default Behavior | Deny inbound, allow outbound | Allow all inbound and outbound |

---

# Stateful vs Stateless

## Security Group — Stateful
If inbound traffic is allowed, return traffic is automatically allowed.

Example:
```text
Allow inbound SSH on Port 22
