## AWS Elastic Beanstalk performs an in-place update when you update your application versions, your application might become unavailable to users for a short period of time. To avoid this, perform a blue/green deployment. To do this, deploy the new version to a separate environment, and then swap the CNAMEs of the two environments to redirect traffic to the new version instantly.

A blue/green deployment is also required if you want to update an environment to an incompatible platform version. For more information, see Updating your Elastic Beanstalk environment's platform version.

Blue/green deployments require that your environment runs independently of your production database, if your application uses one. If your environment includes a database that Elastic Beanstalk created on your behalf, the database and connection of the environment isn't preserved unless you take specific actions. 


echo "# Elastic-BeanStalk-Blue-Green-Deployment" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Asma09Akram/Elastic-BeanStalk-Blue-Green-Deployment.git
git push -u origin main
