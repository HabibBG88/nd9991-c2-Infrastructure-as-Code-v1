### Project Title - Deploy a high-availability web app using CloudFormation
This folder provides the starter code for the "ND9991 - C2- Infrastructure as Code - Deploy a high-availability web app using CloudFormation" project. This folder contains the following files:


#### final-project-starter.yml
Students have to write the CloudFormation code using this YAML template for building the cloud infrastructure, as required for the project. 

#### server-parameters.json
Students may use a JSON file for increasing the generic nature of the YAML code. For example, the JSON file contains a "ParameterKey" as "EnvironmentName" and "ParameterValue" as "UdacityProject". 

In YAML code, the `${EnvironmentName}` would be substituted with `UdacityProject` accordingly.


### Habib work
In this yml template I deployed a VPC, with public and private subnets  across two AZ. 
    
I deployed an Internet Gateway, with a default route on the public subnets, a NAT Gateways for each AZ and default routes in the private subnets.
    
I deploys and configures the web servers on each private subnet (min 4 and max 5)

See screenshot folder for the output name of instances (VPC,RT,LB) and you can find that I added HTTP in front of the DNS name, it will also show an URL saying “Udacity Demo Web Server Up and Running!”

*** url link to the website:  http://iacpr-webap-1j2f59y6ne6ba-999401657.us-east-1.elb.amazonaws.com/

###added after review:
-Bastion host
-S3 bucket with permission
-EC2 InstanceTypeParameter 
-URL to the website

