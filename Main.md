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
