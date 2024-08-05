![Alt text](/Host_Static_Website_with_Ansible.png)

I hosted a Static Website on AWS, for a DevOps project. Used Ansibe server as deployment option. Utilized the following resources. Have also created a GitHub repository with the reference diagram.

1.	Prerequisite – install Git and Visual Studio Code on your computer, and register for a GitHub account
2.	Create VPC with public and private subnets in 2 availability zones
3.	Create Resources such as Nat Gateway,  Bastion Host, and Application Load Balancer in public subnets
4.	Create the security groups
5.	Create two Key Pairs on your computer (one with PuTTy Gen, another with CMD ssh-keygen)
6.	Import to AWS console, two public keys generated with different methods mentioned above. We will call the public key generated with CMD ssh-keygen, Ansible server public key
7.	Add the Ansible server public key into GitHub
8.	We will use the Bastion Host to connect to the Ansible server in the private subnet
9.	Ansible server – this is the EC2 instance we will install Ansible on
10.	Webservers – these are the EC2 instances that will host our website
11.	Add the private key into the Ansible server. Private key for communication between Ansible server, and Webservers
12.	Test the connection between the Ansible Server and the Webservers
13.	Create a GitHub Repository to store the Ansible playbooks
14.	Clone the GitHub repository on Ansible server
15.	Clone the GitHub repository on My PC
16.	Install Ansible on Ansible server
17.	Create the Ansible inventory file in PC repository, and push it to GitHub
18.	Use Ansible to ping the Webservers to test connection
19.	Create the Ansible config file in PC repository and push it to GitHub
20.	Create the Ansible playbook in PC repository and push it to GitHub
21.	Create Application Load Balancer that is used to distribute web traffic to EC2 instances in multiple AZs
22.	Use Route 53 to register domain name, and create a record set
23.	Use AWS Certificate Manager to issue SSL certificate in order to secure web communication to the website
