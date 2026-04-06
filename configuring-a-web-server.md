## Configuring an AWS Web Server

This Document will outline the process of what I have done to create a very simple web server using an EC2 AWS Instance.

## Creating the VM

Before we can get our server configured, we will need to create the Virtual Machine that it will run on. For this, I am using an EC2 AWS Instance which can be found by signing in to the AWS admin console, going to services, and selecting EC2.

Now we will be in the configuration panel for this VM, and I will be using the following settings:
(Insert Images)

This server is being made in a way where it can be experimented with, and be intentionally vulnerable so I can demonstrate the issues that can arise with creating a server on AWS. For example, allowing SSH traffic from any IP could be a security issue as it would allow anyone to connect to the Virtual Machine if they were able to gain access to my SSH key pair.


