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

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/3df63cc4-85af-46b9-9d41-a3423582b065)

* Scroll down to Managed platform updates section.

* Uncheck the Managed updated checkbox

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/58a49240-b22e-4c3e-bc6a-6294d107a5d2)

* Once the my_application_blue_env is provisioned, you will get a page with Health status as ok and with a Domain for the environment.

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/0620ba10-83bf-4725-94ea-059ce9c77cc5)

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/82a8740b-77e3-4a36-9cf1-f4b2e68f12a6)

### Task 4: Creating Elastic Beanstalk Green Environment

The green environment is an identical parallel environment running a different or updated version of the application. This environment allows users to deploy their code changes and test them separately from the blue environment, ensuring that the new version functions correctly before swapping the Domains.

4.1 Click on the Application name to see the environments present.
There will be two environments.

4.2 click on Create new environment button.
* Click on the Configure Environment page :
* Select the Web server environment.
* Enter Environment name as myapplication-green-env

4.3 In the Platform, under Managed platform, choose Node.js from the dropdown.
![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/4ea84cf5-740a-45aa-9230-b6ee75cecce1)

* In the Platform, under Managed platform, choose Node.js from the dropdown.
  
![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/72c155f6-18dc-4812-8d32-c0896c61bf95)

4.4  Click on Next, in Configure service access select Use an existing service role as aws-elasticbeanstalk-service-role, EC2-Role

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/b4a4df25-4a7f-4dd7-b607-f426305da1fa)


![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/d407597b-d995-49b3-982b-16dc366f997b)

default VPC
![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/d5eb6817-aa77-4518-b2bc-8448774febc3)

4.5 Check the Public IP address checkbox

Check the us-east-1a and us-east-1b subnets checkbox under Instance subnets.

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/a89805e7-2240-4d96-ba51-5ef936288423)

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/23fc12c8-7b3e-4fa9-9b5f-a508fe89018c)

Managed Platform Updates

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/acbe1053-d31d-4c94-9853-5bf4b8c607ee)

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/6df7f841-4e68-4e21-8cf3-271ea2ddc112)

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/d099aa7e-4660-4e75-93c6-196791ec5cd2)

### Task 5: Swapping the Domains from Blue to Green

Now we will execute a Domain swap to reroute traffic from the blue environment to the green environment. By conducting this Domain swap, users can activate the updated version of the application and commence serving live traffic from the green environment. This activity guarantees a smooth transition from the old version to the new version, ensuring no downtime for users.


Now we have two environments, namely myapplication_blue_environment with PHP and Myappgreenenvironment-env with Node.js

Next, we will need to swap the Domains.

In the Elastic Beanstalk application dashboard from Myappgreenenvironment-env, click on Actions and select Swap environment domain.

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/2b29254d-2d03-402d-85ad-02653717665b)

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/44f52a57-c302-4dc5-b5a2-638d545b9ad6)

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/5c2ead76-8ff0-4824-b353-c748d4c545cb)


The swap will take a few seconds to complete. You will see the Successfully completed status under Recent Events.

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/0456d4e9-59cc-4bee-8335-5b0efcd03391)


Once the Swap is completed, note that the Domain of the  Myappgreenenvironment-env has been replaced with that of the myapplication_blue_environment.

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/daec3b1d-87d0-4698-957b-fad1707fd141)

Now Click on the Domain (which was the Domain for the MyApplication-Blue-Environment) and notice the content of Myappgreenenvironment-env instead.

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/9545bf85-3f51-4619-b837-76acb206eb33)

![image](https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment/assets/124654068/35891932-7d99-4080-b983-ca6ee4adcf04)
