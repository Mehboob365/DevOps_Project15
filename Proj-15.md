**AWS CLOUD SOLUTION FOR 2 COMPANY WEBSITES USING A REVERSE PROXY TECHNOLOGY**

We will build a secure infrastructure inside AWS VPC (Virtual Private Cloud) network for a fictitious company  that uses WordPress CMS for its main business website, and a Tooling Website (https://github.com/<your-name>/tooling) for their DevOps team. As part of the company’s desire for improved security and performance, a decision has been made to use a reverse proxy technology from NGINX to achieve this.
Cost, Security, and Scalability are the major requirements for this project. Hence, implementing the architecture designed below, ensure that infrastructure for both websites, WordPress and Tooling, is resilient to Web Server’s failures, can accomodate to increased traffic and, at the same time, has reasonable cost.
  
![image](https://user-images.githubusercontent.com/67065306/136455349-9646ab29-7828-4432-a69b-626caa3a7322.png)
  
  
![image](https://user-images.githubusercontent.com/67065306/136625145-421d6470-e0a5-4154-962a-3aedd3bd44bb.png)

  
 **SET UP A VIRTUAL PRIVATE NETWORK (VPC)**
  
  Will set up a Virtual Private Network (VPC)
  We make reference to the architectural diagram and ensure that your configuration is aligned with it.

  1. Create a VPC
  
  ![image](https://user-images.githubusercontent.com/67065306/136627813-81ddaaf4-fc74-4d7f-a370-147c8f6fcc7f.png)

  2. Create subnets as shown in the architecture
  
  
    
    Create a route table and associate it with public subnets
    
    Create a route table and associate it with private subnets
    
    Create an Internet Gateway
    
    Edit a route in public route table, and associate it with the Internet Gateway. (This is what allows a public subnet to be accisble from the Internet)
    
    Create 3 Elastic IPs
