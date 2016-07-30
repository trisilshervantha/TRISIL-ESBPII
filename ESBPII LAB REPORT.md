# ESBPII Lab 01 #
### IT 13026844 ###
### H.T.S.Lusena ###

## Creating Amazon EC2 Windows Instances In Amazon Cloud ##

### Setp 1 - Chose an Amazon Machine Image ###

> After you signed in to the Amazon web service console launch the Amazon EC2 under COMPUTE.

![](http://i.imgur.com/VkwM1C1.jpg)

> Then  press the button called " Launch Instance " under Create Instance category. 

![](http://i.imgur.com/L5ifZHR.jpg)

>Then press the " Select " button of the title " Microsoft Windows Server 2012 R2 Base - ami-8d0acfed ". 

![](http://i.imgur.com/ghV4qoM.jpg)

### Setp 2 - Choose an Instance Type ###

> Amazon EC2 provides a wide range of instance types suited  to fit different uses.Among them we select General Purpose t2.micro instance. Here you should be noticed that the AMIs is marked as "Free tier eligible."

![](http://i.imgur.com/LMnAIr7.jpg)

> After that press the button called " Configure Instance Details " 

### Setp 3 - Configure The Instance Details ###

> Here we can configure the instance details to suite our preference. You can launch multiple instances as you wish. Follow the directions to select a subnet.

![](http://i.imgur.com/e8Wxc19.jpg)

> After that press the " Add Storage " button.

### Setp 4 - Add Storage for the Instance ###

> In that step we can attach additional EBS volumes and instance store volumes to our instance, but not instance store volumes.

![](http://i.imgur.com/kVJeBVY.jpg)


> After that press the " Tag Instance " button.

### Setp 5 - Tag Instance ###

> A tag consists of a case-sensitive key-value pair. Here do nothing to the instance.
![](http://i.imgur.com/94msMmo.jpg)

> After that press the " Configure Security Group " button.

### Setp 6 - Configure Security Group ###

> A security group is a set of firewall rules that control the traffic for your instance. Here you can add rules to allow specific traffic for your instance. Here do nothing to the instance.

![](http://i.imgur.com/794gWLC.jpg)

> After that press the " Review and Launch " button.

### Setp 7 - Review Instance Launch ###

> Here you can review your instance launch details.
##### Capture 1 #####
![](http://i.imgur.com/oEzefnX.jpg)
> 
##### Capture 2 #####
![](http://i.imgur.com/lX9MdOj.jpg)
> 
##### Capture 3 #####
![](http://i.imgur.com/fstjVPh.jpg)

> After that press the " Launch " button.

### Setp 8 - Create a new key pair ###

> After you press the " Launch " button it will be seen the window of " Select an existing key pair or Create a new key pair"  

![](http://i.imgur.com/zoDNOW2.jpg)

>Then select Create a new Key Pair and give a name for that key pair in the Key pair name field of the Create Key Pair dialog box.
>After that press the " Download Key Pair " button.
>Then it will automatically download the " Trisil.pem " file extension key pair file.
>
![](http://i.imgur.com/y63jCOF.jpg)

> Then press the " Launch Instance " button.

### Setp 9 - Launch Status ###

> This is a confirmation page which lets you know to that your instance is running.

![](http://i.imgur.com/PWpVr41.jpg)

> Then press the " View Instance " button.

### Setp 10 - Launch Instance ###

> On the Instances screen, you can view the status of the launch. When you launch an instance, its initial state is pending. Then it will move to the state of running.

![](http://i.imgur.com/LxZnCld.jpg)

### Setp 11 - Download Remote Desktop File ###

> Wait for few minutes to be ready the instance. Then select your running instance and press " Connect " button.

![](http://i.imgur.com/Rn6ybBg.jpg)
 
> After that press " Get Password " button.

### Setp 12 - Connect to Your Instance - Get Password ###

> In this window select your downloaded ".pem " extension file to Key Pair Path and choose Open to copy the entire contents of the file into contents box.

![](http://i.imgur.com/fNyjqf3.jpg)

> Then press the " Decrypt Password " button to decrypt  the password.

![](http://i.imgur.com/PFbpDUE.jpg)

### Setp 13 - Connect to Your Instance - Download Remote Desktop File ###

> When you press the " Decrypt Password " button, a console will display the default administrator password for the instance in the " Connect To Your Instance dialog box " 

![](http://i.imgur.com/BMbIVhL.jpg)

Then press the " Download Remote Desktop File " button.

### Setp 14 - Connect to Remote Desktop ###

> Keep the default administrator password in a safe place.You need this password to connect to the instance.
> Choose Download Remote Desktop File and double clicked it.

![](http://i.imgur.com/OdO2v9Z.jpg)

> Enter the default administrator password and press " OK " button.
> Then it will prompt some kind of a warning window like below one and press " Yes "

![](http://i.imgur.com/L7YSAhA.jpg)

### Setp 15 - Connect to Windows Server ###

> Finally you can connect your Windows Server Instances In Amazon Cloud.

![](http://i.imgur.com/ppGEl2U.png)

### Setp 16 - Terminate the Instance ###

> Finally you have to terminate your created instance Windows Server Instances on Amazon Cloud. 
> For that select the running instance right click on it an goes to Instance State and click Terminate. 

![](http://i.imgur.com/897243C.jpg)


# ESBPII Lab 02 #
### IT 13026844 ###
### H.T.S.Lusena ###

## Creating Amazon EC2 Linux Instances In Amazon Cloud ##

### Setp 1 - Chose an Amazon Machine Image ###

> After you signed in to the Amazon web service console launch the Amazon EC2 under COMPUTE.

![](http://i.imgur.com/VkwM1C1.jpg)

> Then  press the button called " Launch Instance " under Create Instance category.

![](http://i.imgur.com/L5ifZHR.jpg)

>  Then press the " Select " button of the title " Amazon Linux AMI 2016.03.3 (HVM), SSD Volume Type - ami-7172b611 ".

![](http://i.imgur.com/IcFbzwn.jpg) 

### Setp 2 - Choose an Instance Type ###

> Amazon EC2 provides a wide range of instance types suited  to fit different uses.Among them we select General Purpose t2.micro instance. Here you should be noticed that the AMIs is marked as "Free tier eligible."

![](http://i.imgur.com/ZBbclhY.jpg)

> After that press the " Review and Launch " button.

### Setp 3 - Review Instance Launch ###

> Here you can review your instance launch details.
#####Capture 1#####
![](http://i.imgur.com/ZmWmWPO.jpg)
#####Capture 2#####
![](http://i.imgur.com/7EQYzXy.jpg)
#####Capture 3#####
![](http://i.imgur.com/kMuEP44.jpg)
> After that press the " Launch " button.

### Setp 4 - Create a new key pair ###

> After you press the " Launch " button it will be seen the window of " Select an existing key pair or Create a new key pair".
> Then select Create a new Key Pair and give a name for that key pair in the Key pair name field of the Create Key Pair dialog box. 
> 
![](http://i.imgur.com/V5sHZJ3.jpg)

>After that press the " Download Key Pair " button.
>Then it will automatically download the "TrisilLinux .pem " file extension key pair file.

![](http://i.imgur.com/jmL9EE0.jpg)
> Then press the " Launch Instance " button.

### Setp 5 - Launch Status ###

> This is a confirmation page which lets you know to that your instance is running.

![](http://i.imgur.com/AzC29Xr.jpg)

> Then press the " View Instance " button.

### Setp 6 - Launch Instance ###

> On the Instances screen, you can view the status of the launch. When you launch an instance, its initial state is pending. Then it will move to the state of running.

![](http://i.imgur.com/Z6DQpqu.jpg)

### Setp 7 - Connect To Your Instance ###

> Wait for few minutes to be ready the instance. Then select your running instance and press " Connect " button.
> > Then you will be seen " Connect To Your Instance" Window.

![](http://i.imgur.com/H7ohQOR.jpg)


### Setp 8 - Generate the private key using PUTTY Key Generator ###
> Open the PUTTY Key Generator Software. Then press " Load " button. After that select the downloaded " TrisilLinux .pem " file.

![](http://i.imgur.com/8ozBnU2.jpg)

>Then you will get the successful message. Press " OK ".

![](http://i.imgur.com/6oaz6PC.jpg)

> Press the " Save Private Key " button in PUTTY Key Generator.Press " Yes " to the PUTTY warning message.

![](http://i.imgur.com/65EWwZx.jpg)
> Give a name to it " trisillinuxppk " and save it.

![](http://i.imgur.com/7xJkNB6.jpg)


### Setp 9 - Configure the generated private key using PUTTY Configuration ###
> Open the PUTTY Configuration Software. Copy your Public DNS and paste it to the Host Name(or IP Address section) under Session category in PUTTY Configuration.

![](http://i.imgur.com/FJCo3wg.jpg)

> Copy the " ec2-user " and paste it to the Auto-login username under Connection category in PUTTY Configuration.

![](http://i.imgur.com/O6Pk0av.jpg)

> Then go to Auth which in inside the SSH under Connection category in PUTTY Configuration and brouse the " trisillinuxppk " and press " Open " button in PUTTY Configuration window.

![](http://i.imgur.com/6wt7Xw8.jpg)

### Setp 10 - Connect to Amazon Linux AMI ###
Then you will be seen PUTTY security alert and press " YES ".

![](http://i.imgur.com/Tavv2EB.jpg)

> Finally you will have the Amazon Linux AMI window.

![](http://i.imgur.com/nx4c1Qc.jpg)



# ESBPII Lab 03 #
### IT 13026844 ###
### H.T.S.Lusena ###

## Creating instance of MySQL using Amazon RDS and Connect to it using MySQL Workbench Tool ##

### Setp 1 - Chose an Amazon Machine Image ###
> After you sign in to the Amazon Web Services console launch the Amazon RDS under DATABASE.

![](http://i.imgur.com/SfmcIEF.jpg)

> Then press the " Get Started Now " button.

![](http://i.imgur.com/dbaFvea.jpg)

### Setp 2 - Choose an Data Base Instance Type ###

> Amazon RDS provides a wide range of Data base instance types suited  to fit different uses.Among them we choose the " My SQL " tab and the press " Select " button.

![](http://i.imgur.com/GMDjO73.jpg)

### Setp 3 - Select the Production Type ###
> Here we select the MY SQL Free Usage Tier and pres "Next Step " button.

![](http://i.imgur.com/zy16xUZ.jpg)

### Setp 4 - Specify DB Details ###

> Here you have to select db.m1.small- 1 vCPU, 1.7 GiB RAM

![](http://i.imgur.com/3dy8b7S.jpg)

>Fill the database instance settings details and press " Next Step " button. 

![](http://i.imgur.com/mZrykIC.jpg) 

### Setp 5 Configure Advanced Settings ###

> Give the VPC security group as default(VPC) then give a name to database.

![](http://i.imgur.com/qmwbNRD.jpg)

![](http://i.imgur.com/hC6PhNM.jpg)
> Press "Launch DB Instance " button.

> Then press the " View Your DB Instance " button.
![](http://i.imgur.com/8VGCVkO.jpg)

### Setp 6 DB Instance Availability ###

> Now your database instance is available.

![](http://i.imgur.com/Ejmwbhy.jpg)

### Setp 7 Create Security Groups ###

> Press the Security Group tab.

![](http://i.imgur.com/ksGIKPe.jpg)

>Goto EC2 Management Console

![](http://i.imgur.com/qdYUgco.jpg)

> The select " Create Security Group " button

![](http://i.imgur.com/yySHwO5.jpg)

> Then press the "Create " button

![](http://i.imgur.com/QTiFBnH.jpg)


### Setp 8 Conect to MY SQL ###

![](http://i.imgur.com/YqIIWOo.jpg)