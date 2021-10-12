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
  
  ![image](https://user-images.githubusercontent.com/67065306/137033087-47f4b85e-ba38-423b-b8d5-fe6253a83b39.png)

    
  3. Create a route table and associate it with public subnets
  
  ![image](https://user-images.githubusercontent.com/67065306/137033035-543a2262-42e6-45b6-8294-d9b9d7516e17.png)

    
  4. Create a route table and associate it with private subnets
  
  ![image](https://user-images.githubusercontent.com/67065306/137033489-b7cd7b57-98d1-4f92-829a-c92695381902.png)

  ![image](https://user-images.githubusercontent.com/67065306/137033533-8231ef84-b855-4578-b5ad-5949b16dda16.png)

    
  5. Create an Internet Gateway
  
 ![image](https://user-images.githubusercontent.com/67065306/137033662-e570c753-a550-469b-94af-c64a7aa7b4a1.png)
  
  Edit a route in public route table, and associate it with the Internet Gateway. (This is what allows a public subnet to be accisble from the Internet)

 ![image](https://user-images.githubusercontent.com/67065306/137033742-0c89255e-e489-4775-8b16-b9bdceeeea84.png)

    
  6. Create 3 Elastic IPs
  
  
  
  
