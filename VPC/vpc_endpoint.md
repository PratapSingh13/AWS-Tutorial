# VPC End-point

VPC Endpoint enables you to privately connect to your VPC to supported AWS services. Instances  in you VPC do not require public IP addresses to communicate with the resources in the service. 

**Topics**
+ [Purpose of VPC EndPoint](#purpose-of-VPC-endpoint)
+ [Need of VPC EndPoint](#need-of-vpc-endpoint)

## Purpose of VPC EndPoint<a name="purpose-of-VPC-endpoint"></a>

If you want to use your AWS resorces without go to the Internet so this is possible via two ways 
1. Using NAT gateways
2. VPC Endpoint

## Need of VPC EndPoint<a name="need-of-vpc-endpoint"></a>
Till now what we did that we created VPC and NAT gateway and connected NAT with public subnet, if anyone wants to connect with private instance or wants to go on internet using private instance then we have to go from using NAT Gateway. But the problem with NAT Gateway is it is very costly you have to pay huge amount for data transfer via NAT gateway. But here VPC endpoint is completely free you have to pay for only data transfer and that is very minimal charge.



### Contributors
[![Yogendra Pratap Singh][yogendra_avatar]][yogendra_homepage]<br/>[Yogendra Pratap Singh][yogendra_homepage] 

  [yogendra_homepage]: https://github.com/PratapSingh13
  [yogendra_avatar]: https://img.cloudposse.com/75x75/https://github.com/PratapSingh13.png