AWS Networking (VPC)

can launch AWS resources in a logically isolated virtual network that you've defined. This virtual network closely resembles a traditional network that you'd operate in your own data center, with the benefits of using the scalable infrastructure of AWS.

## VPC Dashboard
<details><summary>Virtual Private Cloud</summary>your vpcs <br> Subnets <br> Route tables <br> internet Gateways <br> Egress-only internet gateways <br> DHCP option sets <br> Elastic IPs <br> Managed prefix lists <br> Endpoints <br> Endpoint Services <br>NAT Gateways <br> Peering connections</details>
<details><summary>Security </summary>Network ACLs<br>Security Groups</details>
<details><summary>DNS firewall </summary>Rule groups <br> Domain lists</details>
<details><summary>Network Firewall</summary>Firewalls <br> Firewall policies <br> Network Firewall rule groups <br> TLS inspection configurations<br> Network firewall resource groups </details>
<details><summary>Virtual Private Network (VPN) </summary>Customer gateways <br> Virtual Private gateways <br> site-to-site VPN connections <br> Client VPN endpoints</details>
<details><summary>AWS Verified Access</summary>Verified Access instances <br> Verified Access trust providers <br> Verified Access Groups <br> Verified Access endpoints</details>
<details><summary>Transit Gateways </summary>Transit gateways <br> Transit gateway attachments <br> Transit gateway policy tables <br> Transit gateway route tables <br>Transit gateway multicast</details>
<details><summary>Traffic Mirroring</summary>Mirror sessions<br> Mirror Targets <br>Mirror filters</details>

# features

# Getting started

# working with Amazon VPC

# Pricing

# How VPC works

A subnet is a range of IP addresses in your VPC. You can launch AWS resources into a specified subnet . each subnet must reside entirely within one AZ and cannot span zones.


A route table consists of set of rules, called routes. That are used to determine where network traffic from your subnet or gateway is directed. Use a public subnet for internet connected resources and a private subnet for resources not connected to the internet.


NAT gateway is a network address translation (NAT) service. With NAT gateway, instances in a private subnet can connect to services outside your VPC external services cannot initiate a connection with those instances.

An internet gateway serves two purpose:
  - provide a target in your VPC route tables for internet routable traffic
  - Perform network address Translation (NAT) for instances taht have been assigned public IPV4 Address.

An internet gateway supports IPV4 and IPV6 traffic. It does not cause availability risks or bandwidth constraints on your network traffic. there's no additional change for having an internet gateway in your account.

Secuity groups are stateful, for ex: if you send  a request from an instance the response traffic for that request is allowed to reach the instance regardless of the inbound security group rules. Response to allowed inbound traffic are allowed to leave the instance, regardless of the outbound rules.


To deploy a working internet gateway the following must be completed.
1. The internet gateway must be attached to a VPC
2. Route tables associated with your public subnet must have a route to your internet gateway
3. Any istances in the VPC must have a public IP or elastic IP address assigned.



[To Know More about VPC click here](https://docs.aws.amazon.com/vpc/)
