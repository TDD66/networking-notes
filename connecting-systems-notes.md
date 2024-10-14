# Virtual Private Cloud

**Public Cloud**: 
A public cloud is defined by Microsoft as computing services offered by third party providers over the public internet, they are available to anyone who wants to use or purchase them.

**Private Cloud**: 
A private cloud is a model where all the cloud resources are dedicated to a single user. This is called single-tenancy.

## Virtual Private Cloud
A virtual private cloud is a private cloud that is within a public cloud. A VPC isolated despite being hosted within a public cloud. Various technologies are used to isolate VPCs from other resources within the public cloud, these are:

## Subnets
A subnet is a range of IP addresses within your VPC, they are reserved so that they're not available to everyone within the network. These IP addresses are not accessibile via the public Internet, unlike typical IP addresses.

A default AWS VPC comes with an internet gateway and default subnets are public. Instances launched into default subnets have public and private IP addresses but instances launched into non-default subnets only have a private IP address, unless specified. You can enable internet access for an instance launched in a non-default subnet by attaching an internet gateway to that subnet. This allows the user to control which of their computing resources have direct access to the internet.

## VPN
A virtual private network (VPN) uses encryption to scramble traffic that is passed through publicly shared infrastructure and make it invisible to others. This can be used to establish secure connections to external networks.

## VLAN
A local area network (LAN) connects devices together without use of the internet. This allows resources within the VPC to communicate to one another without the traffic passing over the internet.

## Route tables
A route table contains a set of routes that are used to determine where network traffic from your VPC is directed. Each route in a route table specifies a range of IP addresses where you want traffic to go and the gateway, interface or connection through which the traffic is sent.

**Advantages**: 
- VPCs allow users to create a private cloud network environment that is isolated from the public internet.
- VPCs can accomodate for growing business requirements through scaling.
- VPCs provided by AWS or Google Cloud for example, allows users to customise their network for their specific requirements

**Disadvantages**:
- Perhaps an inexperienced user can make an error setting up a VPC and expose resources unintentionally.
- Because VPCs are served by cloud providers they can be expensive, so users should consider all options before going this route.