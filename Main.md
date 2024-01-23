## Task 1 Login to AWS Management Console
## Task 2 Creating an Elastic Beanstalk Application
2.1 Open Elastic Beanstalk by Searching in Services bar
2.2 Click on Create Application

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/0cea33bb-56fd-4c8f-b710-5df1a05c8380)

2.3 Select Web Application and Give any name of your choice

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/a7eefcb0-da02-4ebd-a783-8e6f8e768b6f)

2.4 Scroll down and under Platform select PHP

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/6be12b21-f661-4534-a68e-22fff5d8b1c7)

2.5 Click on Next
2.6 Under Configure Service Access, select Create and use new service role

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/5c184fa0-28e1-47c0-89cf-79d36ff448c4)

2.7 Choose EC2_Role

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/057d7c46-15fc-4656-b1d5-ffeceae6f535)

2.8 Under Set up networking, database, and tags - optional 
* Choose Default VPC

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/9ef25b62-7f51-40cf-a1f1-5a257060f5e5)

* Under Instance Setting, Select Activated Public IP v4 address

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/be2f3353-d1ef-4349-963f-2ee35931fd96)

* Select 1a and 1b Instance subnets, Click on Next
![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/9ea02f2d-dc4c-4c6e-9a3a-9fc666141382)

2.9 Configure instance traffic and scaling, Scroll down and Under Capacity, select t2.micro Instance types

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/c1c2142d-f5be-4048-9af6-69b27c041851)

2.10 Scroll down to to Managed platform updates , Uncheck Managed Updates

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/1b894131-8fe8-435e-b777-60c040678988)

Click on Next, Review and Submit

2.11 Once everything is successfully done, You will be able to see the Application

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/866b92f0-74bf-43cf-b58e-505d4a96657f)


### Task 3 Create Elastic Beanstalk Blue Environment

3.1 Click on Application which got created and Click on Create an Environment

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/21434b0c-ce68-48de-8022-f3fd8ad9b1bd)

3.2 Select Web server environment

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/fc4a3fc7-29d1-4792-a18c-3d6426c8779f)

3.3 Give the Environment Name as MyApplication-Blue-Environment

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/83035399-6977-456a-b3eb-f1f06bc96932)

3.4 Select PHP as Platform 

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/d883e928-110c-4f14-bdf2-505a72642c9b)

3.5 Click on Next, in Configure service access select Use an existing service role as aws-elasticbeanstalk-service-role, EC2-Role

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/f842157a-dd39-4378-a3ec-335a2e2dec93)

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/d11ccc2f-020d-406b-965a-049aced08857)

3.6 Select Default VPC
![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/113ec421-79ab-4aab-aefc-096bb2b5a0da)

* Instance Setting, Public IP Address

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/6196ff39-d621-406f-9a4b-a83993c4e162)

