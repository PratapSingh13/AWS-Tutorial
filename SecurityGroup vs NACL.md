### Scope: Where to apply *Subnet or EC2* ###

Security groups are tied to an instance whereas Network ACLs are tied to the subnet i.e. NACL are applicable at the subnet level, so any instance in the subnet with an assiciated NACL will follow rules of NACL.
That's not the case with security groups, security groups has to be assigned explicitly to the instance. This means any instances within the subnet group gets the rule applied.
If you have many instances, managing the firewalls using Network ACL can very useful. Otherwise, with Security group, you have to manually assign a security group to the instances.

### Stateful or Stateless ###

Security groups are stateful: This means any changes applied to an incoming rule will be automatically applied to the outgoing rule.
e.g. If you allow an incoming port 80, the outgoing port 80 will be automatically opened.

Network ACLs are stateless: This mean any changes applied to an incoming rule will not be automatically applied to the outgoing rule. 
e.g. If you allow an incoming port 80, you would also need to apply the rule for outgoing traffic.

### Rules ###

In case of NACL the rules are applied in the order of their priority, wherein priority is indicated by the number the rule is assigned
In case of security group, all the rules are applied to the instance.

Multiple Subnets can be bound with a single NACL, but one subnet can be bound with a single NACL only, at a time.
Security Groups are associated with an instance of a service. It can be associated with one or more security groups which has been created by user.
