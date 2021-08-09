# What is NACL

- NACL stands for **Network Access Control List** In AWS, NACL controls traffic to or from a subnet according to a set of inbound and outbound rules. This means it represents network level security. For example, an inbound rule might deny incoming traffic from a range of IP addresses, while an outbound rule might allow all traffic to leave the subnet.

- Because NACLs function at the subnet level of a VPC, each NACL can be applied to one or more subnets, but each subnet is required to be associated with one—and only one—NACL.

- When you create a VPC, AWS automatically creates a default NACL for it. You can add and remove rules from a default NACL, but you can't delete the NACL itself.


### Contributors
[![Yogendra Pratap Singh][yogendra_avatar]][yogendra_homepage]<br/>[Yogendra Pratap Singh][yogendra_homepage] 

  [yogendra_homepage]: https://github.com/PratapSingh13
  [yogendra_avatar]: https://img.cloudposse.com/75x75/https://github.com/PratapSingh13.png