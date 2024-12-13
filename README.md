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
![AWS:detail/](/vpc.JPG)
## SECURITY GROUP
### THINGS TO KNOW ABOUT SECURITY GROUP
AWS Security Groups help you secure your cloud environment by controlling
how traffic will be allowed into your EC2 machines. With Security Groups,
you can ensure that all the traffic that flows at the instance level is 
only through your established ports and protocols.
When launching an instance on Amazon EC2, you need to assign it to a 
particular security group. You can add rules to each security group that
allow traffic to or from designated services including associated instances.
### SECURITY GROUPS HAS TWO ROUTE INBOUND AND OUTBOUND
![INBOUND:detail/](/Security_Group.JPG)
![OUTBOUND:detail/](/security_group2.JPG)
