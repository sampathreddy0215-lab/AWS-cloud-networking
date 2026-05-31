# AWS Route Tables

## What is a Route Table?
A Route Table controls where network traffic is directed inside a VPC.

## Important Route
0.0.0.0/0

This route represents internet traffic.

## Internet Gateway
An Internet Gateway allows communication between AWS resources and the internet.

## Public Subnet
A subnet becomes public when:
- It has a route to Internet Gateway
- Route table contains 0.0.0.0/0

## Private Subnet
A private subnet does not have direct internet access.

## Key Learning
Route tables control traffic flow inside AWS networking.

## Internet Gateway and Route Tables

### What is an Internet Gateway (IGW)?

An Internet Gateway (IGW) allows communication between a VPC and the Internet.

### Example Route

0.0.0.0/0 → Internet Gateway

This route sends all Internet traffic to the Internet Gateway.

### Public Subnet

A subnet becomes public when its Route Table contains:

0.0.0.0/0 → Internet Gateway

Result:

* Internet Access = YES

### Private Subnet

A subnet remains private when there is no route to an Internet Gateway.

Result:

* Internet Access = NO

### Traffic Flow

User → Internet → Internet Gateway → Route Table → EC2 Instance

### Key Points

* Route Table directs traffic.
* Internet Gateway provides Internet access.
* Public Subnet has an IGW route.
* Private Subnet does not have an IGW route.
