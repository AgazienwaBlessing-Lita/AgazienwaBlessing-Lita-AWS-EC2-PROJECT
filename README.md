# AgazienwaBlessing-Lita-AWS-EC2-PROJECT
THIS IS A PROJECT DOCUMENTING THE PROCESS OF LAUNCHING AN EC2 INSTANCE AND DEPLOYING APACHE WEB SERVER IN IT.
## AWS HOME PAGE / ENVIRONMENT
Amazon Web Services (AWS) is the world-leading cloud 
technologies that help any organization and any individual build 
solutions to transform industries, communities, and lives for the better.
Whether they are entrepreneurs launching new businesses, established 
companies reinventing themselves, non-profits working to advance their
missions, or governments and cities seeking to serve their citizens more 
effectively.

![AWS:detail/](/aws_homepage.JPG)
## VPC CREATION
A VPC is a virtual network environment that provides a secure and isolated
space for resources in the AWS cloud. It allows users to: Customize network
configurations, Control traffic, Connect to other resources securely, Isolate
resources, and Enhance security.
### VPCs are made up of components like:
* Subnets
* Route tables
* Security groups
* Network ACLs
* Internet and VPN gateways
* Peering connections.
I used the vpc created by our instructors which is Lita_Project_Vpc because we have reached the number
of vpc's to be created in AWS for free.
### HOW TO CREATE VPC
* sign in to your amazon console
* select region
* search vpc
* click on create vpc
* fill in the requir informations

## WHAT IS AN NACL
Network Access Control List (NACL) is an optional security layer in Amazon
Web Services (AWS) that controls traffic entering and exiting a subnet. NACLs
work like a firewall, and can be used to add an extra layer of security to a VPC.
One of the tools in the AWS security toolkit for enabling defense-in-depth, is the
Network Access Control List (NACL). A NACL is a security layer for your VPC, that 
acts as a firewall for controlling traffic in and out of one or more subnets.
### HOW TO CREATE A PRIVATE NACL
* fill your name
* select private NACL
* fill in your inbound rules, subnet and save changes.

![AWS:detail/](/vpc.JPG)

## SECURITY GROUPS
### THINGS TO KNOW ABOUT SECURITY GROUP
AWS Security Groups help you secure your cloud environment by controlling
how traffic will be allowed into your EC2 machines. With Security Groups,
you can ensure that all the traffic that flows at the instance level is 
only through your established ports and protocols.
When launching an instance on Amazon EC2, you need to assign it to a 
particular security group. You can add rules to each security group that
allow traffic to or from designated services including associated instances.

### HOW TO CREATE SECURITY GROUPS
* select your region
* search security group
* click on create security group
* fill in your basic details
* set your inbound and outbound rulesclick on create security groups
Outbound: traffic that is leaving the router
Inbound: traffic that is entering the router

![INBOUND:detail/](/Security_Group.JPG)
![OUTBOUND:detail/](/Security_Group2.JPG)

## CREATION OF KEY PAIR
An AWS key pair is a set of security credentials that consists of a public
key and a private key. You use key pairs to: 
* Prove your identity when connecting to an Amazon EC2 instance 
* Encrypt and decrypt login information 
* Securely access and manage EC2 instances 
### STEPS I USED TO DOWNLOAD MY KEY PAIR
* Open the Amazon EC2 console 
* Select Key Pairs under Network & Security in the navigation pane 
* Choose Create Key Pair 
* Give your key pair a name 
* Choose the key pair file format (.pem)
* Clicking Create Key Pair 

![key pair:detail/](/key_pair.JPG)

## LAUNCHING MY INSTANCE IN AWS
Launching an instance in AWS (Amazon Web Services) means creating a virtual
server in the AWS cloud. 
### STEPS TO LAUNCH YOUR INSTANCE IN aws
* Log in to your AWS account
* Open the EC2 dashboard
* Click Launch Instance
* Name your instance and add tags
* Choose an Amazon Machine Image (AMI)
* Select an instance type
* Configure key pairs
* Configure network settings
* Configure storage
* check if everything is correct
* Launch your instance 

![INSTANCE:detail/](/instance.JPG)
![INSTANCE:detail/](/instance_1.JPG)
![INSTANCE:detail/](/instance_2.JPG)
![INSTANCE:detail/](/instance_3.JPG)
![INSTANCE:detail/](/instance_4.JPG)

## INSTALLING APACHE
Apache is a free, open-source software technology that can be used in AWS
for a variety of purposes, including: 
### Apache Web Server
    A free, open-source web server that delivers web contentover the internet,
    You can install the Apache web server on an EC2 instance
### Apache Cassandra
    An open-source, NoSQL database designed for applicationsthat require fast 
    read and write performance. You can use Amazon Keyspaces to run Cassandra
    workloads. 
### Apache Spark
    An open-source, distributed processing system used for big dataworkloads. 
    It supports code reuse across multiple workloads, including batch processing,
    interactive queries, real-time analytics, machine learning, and graph processing. 
### Apache Hadoop
    An open-source framework that is used to efficiently store and process large datasets
### Apache Flink
    Can process both unbounded (streams) and bounded (batches) data sets. 
### Apache MXNet
    A machine learning inference framework.
### Apache Iceberg
    An open table format that can scale and evolve seamlessly

### STEPS TO INSTALL APACHE
* click on your EC2 instance 
* click on connecting
* click on ssh client
* open your folder where keypair was downloaded
* right click on the empty space
* select show more option
* select get bash here(your comand window will open)
* copy your bash from your instance page and past
* A prompt will come up, you type "yes"
* type sudo yum update -yes ( pounch enter)
* type sudo yum install httpd -y ( pounch enter)
* copy and past your remaing code

![apache installation:detail/](/kp.JPG)
![apache installation:detail/](/apache_download.JPG)
![apache installation:detail/](/apache_download1.JPG)
![apache installation:detail/](/apache.JPG)

### HOW TO CHECK YOUR TEST PAGE
* go to your EC2 instance
* copy your IP address and past it on your browser and refresh

![test page:detail/](/apache_text_page.JPG)
