# AWS Site-to-Site VPN Troubleshooting Guide

## Overview

AWS Site-to-Site VPN provides secure IPsec connectivity between an on-premises network and an AWS Virtual Private Gateway (VGW) or Transit Gateway (TGW).

## Common Symptoms

- VPN tunnel is DOWN
- Tunnel flapping
- BGP neighbors not establishing
- Traffic not reaching AWS resources
- High latency or packet loss

## Verification Steps

### AWS

- Check tunnel status
- Verify Customer Gateway configuration
- Review Transit Gateway or VGW attachments
- Confirm route propagation

### On-Premises

- Verify IKE Phase 1 status
- Verify IPsec Phase 2 status
- Confirm BGP neighbor state
- Validate static or dynamic routes

## Common Troubleshooting Commands

### Cisco

show crypto isakmp sa
show crypto ipsec sa
show ip bgp summary
show ip route

### Palo Alto

show vpn ike-sa
show vpn ipsec-sa
show routing protocol bgp summary

## Common Root Causes

- Pre-shared key mismatch
- Incorrect IKE/IPsec proposals
- BGP ASN mismatch
- Firewall blocking UDP 500 or UDP 4500
- Missing route propagation
- MTU or MSS issues

## Best Practices

- Configure redundant VPN tunnels
- Use BGP for dynamic routing
- Enable tunnel monitoring
- Document encryption parameters
- Test failover during maintenance windows
