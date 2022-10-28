# Security-Groups
A security group acts as a virtual firewall for your instance to control inbound and outbound traffic. For each security group, you add rules that control the inbound traffic to instances, and a separate set of rules that control the outbound traffic. 

> Note: AWS Security group could only be applied on some instance 

## Inboud
By default security group deny all traffic to the instance, so with the help of inboud rule we can allow some range of IP/Individual Ip/All
to make request on our instance via allowed protocal.



>To restrict VPC to connect only to certain instances, you can specify the security group ID (recommended) or private IP address of the instances that you want to allow. In either case, your security group inbound rule still needs to allow traffic on all ports (0–65535).

## Outbound
Outboud rule basic configured to make request from instance to outside world
### Example
- From one instance to another instance
- From instance to internet 

### Configurables in inbound/outbound rules are :
- Type
- Protocols
- Port Range
- Source 

### Sample rule
| Type| Protocol|Port Range| Source
|:----|:--------|:---------|:-------
|All TCP|TCP|0-65535|10.1.0.0/22