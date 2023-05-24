# Deploying Spring Boot MySQL REST API on AWS Elastic Beanstalk: A Comprehensive Guide


## Step 1: Configure Environment

1.  Navigate to the AWS Elastic Beanstalk console at [https://console.aws.amazon.com/elasticbeanstalk/](https://console.aws.amazon.com/elasticbeanstalk/).
2.  Click on `Create a new environment`.
3.  Select `Web server environment` and click `Select`.
4.  In the `Environment information` section, type `02-rest-api-mysql` as the environment name.
5.  In the `Platform` section, select `Managed platform` and from the dropdown menus, select `Java`.
6.  In the `Application code` section, choose `Upload your code`. Click `Choose file` to select the Spring Boot JAR file from your local computer. Set the `Version label` as `02-rest-api-mysql-source`.
7.  Choose the `Presets` as `Single instance (free tier)`.
8.  Click on **Next**

<br>

![Screenshot 2023-05-24 at 11 35 15 AM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/7f5501ba-18af-48c0-944d-e1ec88549573)

<br>

![Screenshot 2023-05-24 at 11 35 50 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/5ebee113-ddf9-4f0b-86c1-cc56a5768517)

<br>

![Screenshot 2023-05-24 at 11 36 13 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/c70ae4a4-713c-48bb-a61a-56ba02ceaa1e)

<br>

![Screenshot 2023-05-24 at 11 36 36 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/044dc2e9-c01f-4eb5-9de5-c54c95ad8dc5)

<br>

![Screenshot 2023-05-24 at 11 37 08 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/462297da-672b-4efc-9845-4408b8603587)

<br>

![Screenshot 2023-05-24 at 11 37 38 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/7ef5f7d0-56f7-4711-83ce-991359f878f5)

<br>

![Screenshot 2023-05-24 at 11 38 11 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/a231259e-fdb7-49f3-b354-84d824bb4c14)

<br>

## Step 2: Configure Service Access

1.  In the `Service Role` section, choose the `Use an existing service role` option and select your preferred role from the dropdown menu.
2.  In the `Instances` section, choose `Use an existing EC2 instance profile` and select your preferred profile from the dropdown menu.
3.  If you are facing any issue in this page like no service role is showing, you can refer to this doc: https://github.com/amideb/Beanstalk-Instance-Profile-Troubleshooting
4.  Otherwise, Click on **Next**

<br>

![Screenshot 2023-05-24 at 11 38 52 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/d7238c3d-64ec-42fd-b1e5-0adfc263f0d2)

<br>

## Step 3: Set up Networking, Database, and Tags 

1. Scroll down
2. In the `Database` section, click on `Enable Database`. Select `mysql` for Engine. Provide the username and password. 
3. Make Database deletion Policy to `Delete`.
4. Click `Skip to review`.

<br>

![Screenshot 2023-05-24 at 11 39 33 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/a8e773a8-d513-4032-b8ee-99d36f8731d9)

<br>

![Screenshot 2023-05-24 at 11 41 37 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/64a90b86-937c-411c-8410-9bdbf496cdfe)

<br>

![Screenshot 2023-05-24 at 11 43 05 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/ee077b1b-00a5-4839-b3fd-d5fe2ebfe9ed)

<br>


## Step 4: Review

1.  Review all your configurations and if everything is according to your requirements, click on `Submit`.


![Screenshot 2023-05-24 at 11 44 05 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/edcf7152-6da0-49a8-aafb-7f8eb621fd37)

<br>

![Screenshot 2023-05-24 at 11 44 22 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/8f26b554-ae1a-4af3-a69b-7ce754fca8d2)

<br>

![Screenshot 2023-05-24 at 11 44 38 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/cf9e972c-a4c2-4030-8c2d-db10ac1e2259)

<br>


## Step 5: Wait for 10-15 Mins

- AWS Elastic Beanstalk will then automatically handle the deployment, from capacity provisioning, load balancing, and automatic scaling to application health monitoring. After a few minutes, your environment should be up and running.

- Note: The environment URL will be displayed in the AWS Elastic Beanstalk console once the environment is successfully launched. You can use this URL to access your deployed Spring Boot REST API.

<br>

![Screenshot 2023-05-24 at 11 51 34 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/c113eeeb-6944-4c9c-8ada-269c8828d33c)

<br>

## Step 6: Wait is Over

Congratulations, your Spring Boot MySQL REST API is now successfully deployed on AWS Elastic Beanstalk! 🎉🚀

Your application is now running in the cloud and is accessible from anywhere. This is a significant accomplishment that will help drive your project forward. I encourage you to continue exploring and pushing the boundaries of what you can achieve.

Remember, every step forward is a step towards success. Well done! 🙌🥳

<br>

![Screenshot 2023-05-24 at 11 58 30 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/8581c90a-f3a8-4835-a6a7-94b94ecaf041)

<br>

## Step 7: Open the Application

### Congratulations! 🎉

Congratulations on successfully deploying your Spring Boot MySQL REST API on AWS Elastic Beanstalk! 🎉🚀

This is a major achievement and I hope it brings you one step closer to your goals. Keep up the great work and continue to push the boundaries of what you can accomplish! 😃👏

Don't forget to celebrate this moment, you've earned it! 🥳🎊


<br>

![Screenshot 2023-05-24 at 11 59 20 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/5e33c9eb-8662-4e2b-81b3-e6a77188f1f7)

<br>

![Screenshot 2023-05-24 at 11 59 40 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/18ac8bbe-ff61-45e5-92e5-634c159c8d14)

<br>

![Screenshot 2023-05-24 at 11 59 55 PM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/c9a29245-b055-4052-806a-c42924535f8f)

<br>

![Screenshot 2023-05-25 at 12 00 52 AM](https://github.com/amideb/deploy-spring-boot-rest-api-mysql-aws-elastic-beanstalk/assets/57451228/2260322e-8011-4dc6-9954-df6a10f943da)

<br>



#### Remember: AWS resources can incur charges. Make sure to stop or delete resources when you've finished with them to avoid unnecessary costs.
