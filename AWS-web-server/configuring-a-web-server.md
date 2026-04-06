## Configuring an AWS Web Server

This Document will outline the process of what I have done to create a very simple web server using an EC2 AWS Instance.

## Creating the VM

Before we can get our server configured, we will need to create the Virtual Machine that it will run on. For this, I am using an EC2 AWS Instance which can be found by signing in to the AWS admin console, going to services, and selecting EC2.

Now we will be in the configuration panel for this VM, and I will be using the following settings:
![Image of AWS showing name, OS image, and Instance type](images/web-server-01.png)
![Image of AWS showing key pair, Network Settings, Storage](images/web-server-02.png)

This server is being made in a way where it can be experimented with, and be intentionally vulnerable so I can demonstrate the issues that can arise with creating a server on AWS. For example, allowing SSH traffic from any IP could be a security issue as it would allow anyone to connect to the Virtual Machine if they were able to gain access to my SSH key pair.

Now I will configure the security group that the VM belongs in to allow TCP connections on port 8080 from any IP. This will be the port responsible for HTTP communications as using a higher port number because Linux requires additional configuration for lower port numbers.
![Image of AWS showing the inbound rules of the security group the VM belongs to](images/inbound-rules.png)

## Creating Buckets

Now we will create a bucket which will be used for storing any files which will be displayed on the website. The bucket will be configured with the following settings (any omitted settings have been left as their defaults):
![Image of AWS showing bucket name, region, and namespace](images/bucket-creation-01.png)
![Image of AWS showing public access settings](images/bucket-creation-02.png)
