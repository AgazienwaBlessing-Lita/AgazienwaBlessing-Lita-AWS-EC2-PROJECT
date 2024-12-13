# AgazienwaBlessing-Lita-AWS-EC2-PROJECT
 THIS IS PROJECT DOCUMENTING THE PROCESS OF LAUNCHING AN EC2 INSTANCE AND DEPLOYING APACHE WEB SERVER IN IT.
### AWS HOME PAGE / ENVIRONMENT
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
1. Subnets
2. Route tables
3. Security groups
4. Network ACLs
5. Internet and VPN gateways
6. Peering connections.
I used the vpc created by our instructors which is Lita_Project_Vpc because we have reached the number
of vpc's to be created in AWS for free.
### HOW TO CREATE VPC
1. select region
2. 

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
1. select your region
2. search security group
3. click on create security group
4. fill in your basic details
5. set your inbound and outbound rulesclick on create security groups
### SECURITY GROUPS HAS TWO ROUTE INBOUND AND OUTBOUND

![INBOUND:detail/](/Security_Group.JPG)
![OUTBOUND:detail/](/Security_Group2.JPG)

## CREATION OF KEY particular
An AWS key pair is a set of security credentials that consists of a public
key and a private key. You use key pairs to: 
1. Prove your identity when connecting to an Amazon EC2 instance 
2. Encrypt and decrypt login information 
3. Securely access and manage EC2 instances 
### STEPS I USED TO DOWNLOAD MY KEY PAIR
1. Open the Amazon EC2 console 
2. Select Key Pairs under Network & Security in the navigation pane 
3. Choose Create Key Pair 
4. Give your key pair a name 
5. Choose the key pair file format (.pem)
6. Clicking Create Key Pair 

![key pair:detail/](/key_pair.JPG)

## LAUNCHING MY INSTANCE IN AWS
Launching an instance in AWS (Amazon Web Services) means creating a virtual
server in the AWS cloud. 
### STEPS TO LAUNCH YOUR INSTANCE IN aws
1. Log in to your AWS account
2. Open the EC2 dashboard
3. Click Launch Instance
4. Name your instance and add tags
5. Choose an Amazon Machine Image (AMI)
6. Select an instance type
7. Configure key pairs
8. Configure network settings
9. Configure storage
10. check if everything is correct
11. Launch your instance 

![INSTANCE:detail/](/instance.JPG)
![INSTANCE:detail/](/instance_1.JPG)
![INSTANCE:detail/](/instance_2.JPG)
![INSTANCE:detail/](/instance_3.JPG)
![INSTANCE:detail/](/instance_4.JPG)

## INSTALLING APACHE
Apache is a free, open-source software technology that can be used in AWS
for a variety of purposes, including: 
1. Apache Web Server: A free, open-source web server that delivers web content
   over the internet. You can install the Apache web server on an EC2 instance
2. Apache Cassandra: An open-source, NoSQL database designed for applications
   that require fast read and write performance. You can use Amazon Keyspaces to 
   run Cassandra workloads. 
3. Apache Spark: An open-source, distributed processing system used for big data
   workloads. It supports code reuse across multiple workloads, including batch 
   processing, interactive queries, real-time analytics, machine learning, and 
   graph processing. 
4. Apache Hadoop: An open-source framework that is used to efficiently store and 
   process large datasets
5. Apache Flink: Can process both unbounded (streams) and bounded (batches) data sets. 
6. Apache MXNet: A machine learning inference framework.
7. Apache Iceberg: An open table format that can scale and evolve seamlessly

### STEPS TO INSTALL APACHE
1. click on your EC2 instance 
2. click on connecting
3. click on ssh client
4. open your folder where keypair was downloaded
5. right click on the empty space
6. select show more option
7. select get bash here(your comand window will open)
8. copy your bash from your instance page and past
9. A prompt will come up, you type "yes"
10. type sudo yum update -yes ( pounch enter)
11. type sudo yum install httpd -y ( pounch enter)
12. copy and past your remaing code

![apache installation:detail/](/kp.JPG)
![apache installation:detail/](/apache_download.JPG)
![apache installation:detail/](/apache_download1.JPG)
![apache installation:detail/](/apache.JPG)

## HOW TO CHECK YOUR TEST PAGE
1. go to your EC2 instance
2. copy your IP address and past it on your browser and refresh

![test page:detail/](/apache_text_page.JPG)
