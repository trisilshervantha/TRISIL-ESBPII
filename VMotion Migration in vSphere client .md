# ESBPII Lab 07 #
### IT 13026844 ###
### H.T.S.Lusena ###

## VMotion Migration in vSphere client.  ##

### Hardware requirements. ###

> 1. From the outside world perspective, there should be a switch which connects 
     two virtual machines. 
> 2. Gigabit or faster Ethernet network connection.
> 3. Compatible CPUs.
> 4. Access to the same physical network.

### Software requirements. ###

> 1. Shared storage between 2 virtual machines to store the virtual machine’s         files.
> 2. Network called vMotion Network (private, non-routed, gigabit faster) between two host which involves in vMotion.
> 3. Production Network   to have identical network port groups for two virtual machines.


### Advantages of VMotion ###

> 1. Can move powered on machine on place to another virtually.
> 2. Where you want striving to balance the load of virtual machine to cross different hosts.  It improves overall hardware utilization.
> 3. Network called vMotion Network (private, non-routed, gigabit faster) between two host which involves in vMotion.
> 4. Production Network   to have identical network port groups for two virtual machines.


### Disadvantages of VMotion ###

> 1. If your virtual CD Roms are connected to a piece of physical medium actual Disks they reside in the host and that will block the vMotion migration.
> 2. If you use ISO and if you place it for your local data store or private data store in can only be seen by one host. It will block the VMotion Migration.
> 3. A virtual machine must not have CPU affinity configured for VMotion purpose.


### Setp 1 - Create the shared storage to do VMotion. ###
> Before change the VMs and Templates.
> ![](http://i.imgur.com/AaPK5dy.jpg)

Then change the VMs and Templates into Hosts and Clusters.
![](http://i.imgur.com/GcXqOz8.jpg) 

### Setp 2 - Create the VM Kernel Port on each host. ###
> Select the Configuration Tab and then select the Networking Adapters and see the visibility of the new connection.
![](http://i.imgur.com/69SGPxL.jpg)

### Setp 3 - Create a new Virtual Switch. ###
> Then select the Networking which is under Hardware.
> Click on Add Networking to create a new Virtual Switch.
![](http://i.imgur.com/9OmvD3M.jpg)

### Setp 4 - Create a VMKernel on new Switchv. ###
> To create a VMKernel on that new Switch select VMKernel  and click on Next.
![](http://i.imgur.com/sSRq8vZ.jpg)

### Setp 5 - Select a vmnic. ###
> Select a vmnic which is used to transmit the VMTraffic through VM Network and press Next button.
![](http://i.imgur.com/vZxGbzQ.jpg)


### Setp 6 - Set the Port Properties. ###
> Fill the Network Lable as vMotion and VLan ID as None(0).
> We set Use this port group for vMotion and click on Next. 
![](http://i.imgur.com/1kiLHtW.jpg)

###Step 7 - Set the unique IP address for each host. ###
> We use the following IP settings:
IP Address: 50.50.50.1
Subnet Mask: 255.255.255.252 (Since we will use only 2 ip's). Then click next.

![](http://i.imgur.com/zXBf8pI.jpg)

> Now you can see the summery report of it and click Finish Button. Now we have set a VMotion port for a one host.
![](http://i.imgur.com/ywxkBg5.jpg)

###Step 8 - Configure the other Virtual machine's VMotion Port. ###

> Here you have to do the step 3 to step 7 for the other Virtual machine.
>> Step 8.1 Click on Add Networking to create a new Virtual Switch.
![](http://i.imgur.com/9OmvD3M.jpg)

>> Step 8.2 To create a VMKernel on that new Switch select VMKernel  and click on Next.
![](http://i.imgur.com/sSRq8vZ.jpg)

>> Step 8.3 Select a vmnic which is used to transmit the VMTraffic through VM Network and press Next button.
![](http://i.imgur.com/vZxGbzQ.jpg)

>> Step 8. 4 Fill the Network Lable as vMotion and VLan ID as None(0).
>> We set Use this port group for vMotion and click on Next. 
![](http://i.imgur.com/1kiLHtW.jpg)

>> Step 8. 5 We use the following IP settings:
IP Address: 50.50.50.2
Subnet Mask: 255.255.255.252 (Since we will use only 2 ip's). Then click next.
![](http://i.imgur.com/I2Vwvo2.jpg)

>> Now you can see the summery report of it and click Finish Button. Now we have set a VMotion port for a one host.
![](http://i.imgur.com/ywxkBg5.jpg)

###Step 9 - Select a running Virtual Machine to migrate. ###
![](http://i.imgur.com/q9cfZCk.jpg)
> In the above picture we can see that EXSI 02 has four virtual machines and we have to select a running virtual machine (1st one) to migrate to EXSI 01.


###Step 10 - Migrate a virtual machine. ###
> Right click on the running virtual machine (1st one) and select migrate.
![](http://i.imgur.com/9f1QU0W.jpg) 

> VMotion Migration involves change host. So keep the tick on that one and press Next button.
![](http://i.imgur.com/hCZPyKn.jpg)


###Step 11 - Migrate a virtual machine - Select the destination. ###

> Here we have to select the target destination where we will move the virtual machine that is EXSI 01. The important thing is when you select the destination it should give "Validation Succeeded" message. 
> Then press Next button.
![](http://i.imgur.com/Yo2JsQx.jpg)

###Step 12 - Migrate a virtual machine - Set the priority. ###

> Select High Priority and press next button.
![](http://i.imgur.com/xPX0rr0.jpg)


###Step 13 - Migrate a virtual machine - Summery. ###

> Here you can see the summery of the VMotion. Press Finish button.
![](http://i.imgur.com/LTBTMZb.jpg)

> Now we can see the migration began.
![](http://i.imgur.com/IKNMZ4w.jpg)

> After complete the migration we can see that Virtual machine is running on EXSI 01.
![](http://i.imgur.com/NWNO4Xc.jpg)
