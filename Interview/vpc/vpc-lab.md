# Let's learn how to create VPC and other networking modules

**Step-1.0** Search for VPC in search box

![](images/vpc-1.1.png)

**Step-1.1** Or go to **Services**

In Services you will find **VPC** in **Networking and Content Delivery**

![](images/vpc-1.2.png)

**Step-1.2** Create VPC

Click on **Create VPC**

![](images/vpc-1.3.png)

**Step-1.3** Put some details

**Name tag -** Here provide the name for you VPC.

**IPv4 CIDR block -** Give CIDR block for your VPC.

**IPv6 CIDR block -** Keep *No IPv6 CIDR block* .

**Tenancy -** Here you need to provide Tenancy as *dedicated* or *default*. If you choose *dedicated* then it will cost you.

*After all this hit on *Create VPC**.

![](images/vpc-1.4.png)

**Step-1.4** Go through to your VPC

Here you will find the *VPC ID* *State* and all state should be *Available*.

![](images/vpc-1.5.png)


**Step-1.5** Find your VPC

Click on *Your VPCs* and you will find the VPC that you made.

![](images/vpc-1.6.png)

**Step-2.0** Create Subnet

Click on **Subnets** in left pane.

![](images/subnet-1.1.png)

Here if you are creating for first time you will find only default subnets which were provided by AWS itself

![](images/subnet-1.2.png)

**Step-2.1** Select VPC

Select VPC where you want to create subnets because subnets are VPC associated, you can not use a subnet in different VPC.

![](images/subnet-1.3.png)

**Step-2.2** Choose **Availability Zone**

Here you need to choose AZ for your subnet

![](images/subnet-1.4.png)

**Step-2.3** Give Subnet CIDR

In this step you need to give subnet CIDR and most important its range should be inside the VPC CIDR.

![](images/subnet-1.5.png)

**Step-2.4** Find your Subnet

Here Your Subnet created successfully.

![](images/subnet-1.6.png)

**Step-3.0** Let's create *Internet Gateway*

Click on **Internet Gateway** on left pane

Here you will find a IGW which could be either on **Attach** or **Detached** mode.

![](images/IGW-1.1.png)

**Step-3.1** Create Internet Gateway

![](images/IGW-1.2.png)

**Step-3.2** IGW created successfully

Here IGW has been created successfully but notice it is in **detached** mode so we need to attach this to my VPC.

![](images/IGW-1.3.png)

**Step-3.3** Attach IGW to VPC

Click on **Attach to VPC** in *Actions* toggle.

![](images/IGW-1.4.png)

**Step-3.4** Select the VPC

Select your Available VPC in which you want to attach IGW

![](images/IGW-1.5.png)

**Step-3.5** IGW attached to VPC

Here you can clear find a difference the it's status is changed  **detached** to **attached**

![](images/IGW-1.6.png)


**Step-4.0** Create **Route Table**

If you click on *Route Table in left pane you will be re-directed to Route Table creation page, and here you will find a Route Table is already created for our newly created VPC that is done by AWS. But We will create a new Route Table so click on **Create Route Table**

![](images/rt-1.1.png)

Here you need to give Name of you route table then select VPC ID in which you want to create route table

![](images/rt-1.2.png)

Here your route table has been created

![](images/rt-1.3.png)

**Step-4.1** Subnet Association

Now you need to associate subnets into your newly created route table, so click on *Subnet associations* at bottom.

![](images/rt-1.4.png)

Choose your subnet which you want to associate

![](images/rt-1.5.png)

And all done.
