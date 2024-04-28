**1.** **What do you mean by VPC in AWS?**

**Answer -** VPC stands for **Virtual Private Cloud**.  It allows you to customize your networking configuration. VPC is a network that is logically isolated from other networks in the cloud. It allows you to have your private IP Address range, internet gateways, subnets, and security groups.

**2.** **What is VPC CIDR?**

**Answer -** When you create a VPC, you must specify a range of IPv4 addresses for the VPC in the form of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0. 0.0/16 . This is the primary CIDR block for your VPC.

**3.** **What are the components of AWS VPC?**

**Answer -** List of components of AWS VPC
- Virtual Private Cloud (VPC)
- Internet Gateway
- NAT Gateway
- Hardware VPN
- Virtual Private Gateway
- Peering Connection
- VPC Endpoint

**4.** **How do you connect VPC to the Internet?**

**Answer -** Internet Gateway enables Amazon EC2 instances in the VPC to directly access the Internet.

**5.** **How many subnets can a VPC have? OR How many subnets can we create per VPC?**

**Answer -** User can create 200 subnets per VPC. If want to create more, need to submit a case at the support center.


**6.** **What is NAT Gateway and tell me it's use case?**

**Answer -** NAT stands for Network Address Translation Gateway it uses to convert private ip into public ip and make forward and vice versa, You can use NAT gateway to enable instances in a Private subnet to connect to the internet.

**7.** **In what type of Subnet you will use NAT Gateway?**

**Answer -** We have to use NAT gateway in and only on **Public Subnet**, but it uses for Private Subnet.

**8.** **What is the most important thing that you need to associate with NAT gateway?**

**Answer -** You need to specify an Elastic IP address to associate with NAT gateway when you create.

**9.** **If I have created a NAT gateway and I associated that with a Private Subnet but now I'm getting error for instance not able to communicate with internet so what will be the possible options for this?**

**Answer -** You associated your NAT gateway with Private Subnet instead of Public Subnet.

**10.** **If I have created a NAT gateway and I associated that with a Public Subnet but somehow my instances are not able to contact with internet so what are the possible solutions you will go for?**

**Answer -**  NAT gateway never get public IP so why we need to give Elastic IP and also I will check on Route Table entry for NAT gateway. 

**11.** **Can Amazon EC2 instances within a VPC communicate with Amazon EC2 instances, not within a VPC?**

**Answer -** Yes. If an Internet gateway has been configured.

**12.** **Can you monitor the network traffic in your VPC?**

**Answer -** Yes. You can use the Amazon VPC Flow Logs feature or CloudWatch and CloudWatch logs to monitor the network traffic in your VPC.

**13.** **Can you use your existing AMIs in Amazon VPC?**

**Answer -** You can use AMIs in Amazon VPC that are registered within the same region as your VPC. For example, you can use AMIs registered in us-east-1 with a VPC in us-east-1.

**14.** **How do you specify which Availability Zone my Amazon EC2 instances are launched in?**

**Answer -** When you launch an Amazon EC2 instance you must specify the subnet on which to launch the instance. The instance will be launched in the Availability Zone associated with the specified subnet.

**15.** **What are the differences between security groups in a VPC and network ACLs in a VPC?**

**Answer -** Security groups in a VPC specify which traffic is allowed to or from an Amazon EC2 instance.

Network ACLs operate at the subnet level and evaluate traffic entering and exiting a subnet. Network ACLs can be used to set both Allow and Deny rules. Network ACLs do not filter traffic between instances in the same subnet.

**16.** **Upto what number of Security Group you can associate for a EC2 instance?**

**Answer -** Upto 5

**17.** **Can you able to deny rule in Security Group?**

**Answer -** No in Security Group you can not deny rule but in NACL you can do this.

**18.** **What is difference between Custom NACL and Default NACL**?

**Answer -** Default NACL allows all inbound and outbound traffic but Custom NACL denies all inbound and outbound traffic untill you add rules.

 

### Contributors
[![Yogendra Pratap Singh][yogendra_avatar]][yogendra_homepage]<br/>[Yogendra Pratap Singh][yogendra_homepage] 

  [yogendra_homepage]: https://github.com/PratapSingh13
  [yogendra_avatar]: https://img.cloudposse.com/75x75/https://github.com/PratapSingh13.png
