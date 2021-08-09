# What is NAT Gateway

- NAT stands for *Network Address Translation* it uses to convert private ip into public ip and make forward and vice versa.

- You can use NAT gateway to enable instances in a Private subnet to connect to the internet although NAT attached with public subnet but it is for private subnet(it is a kind of mediator).

- To create a NAT gateway, you must specify the public subnet in which the NAT gateway should reside.

- You are charged for creating and using a NAT in your account.

- **You must also specify an Elastic IP address to associate with NAT gateway when you create.**

- No need to assign Public IP address to your Private Instances.

- After you have created a NAT gateway you must update the Route Table associated with one or more of your private subnets to point internet bound traffic to the NAT gateway **this enables your private subnet to communicate with internet**

- Deleating a NAT gateway, disassociate it's Elastic IP but does not release Elastic IP from your account. 


### Contributors
[![Yogendra Pratap Singh][yogendra_avatar]][yogendra_homepage]<br/>[Yogendra Pratap Singh][yogendra_homepage] 

  [yogendra_homepage]: https://github.com/PratapSingh13
  [yogendra_avatar]: https://img.cloudposse.com/75x75/https://github.com/PratapSingh13.png