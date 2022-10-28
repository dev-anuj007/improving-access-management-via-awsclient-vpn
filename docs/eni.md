# Elastic Network Interface
An elastic network interface (referred to as a network interface in this documentation) is a logical networking component in a VPC that represents a virtual network card.

Each instance in your VPC has a default network interface (the primary network interface) that is assigned a private IPv4 address from the IPv4 address range of your VPC. You cannot detach a primary network interface from an instance. You can create and attach an additional network interface to any instance in your VPC. The number of network interfaces you can attach varies by instance type. 

### Attaching multiple network interfaces to an instance is useful when you want to:

- Create a management network.

- Use network and security appliances in your VPC.

- Create dual-homed instances with workloads/roles on distinct subnets.

- Create a low-budget, high-availability solution