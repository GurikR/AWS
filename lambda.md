## Why Lambda?

+ EC2 instances should be provisioned
+ Above EC2 instances are limited by their chosen RAM and CPU
+ There should not be any downtime
+ Can be scaled by configuring autoscaling groups

## With Lambda

+ virtual function - all we need to provision the code and no servers to manage
+ great for short executions
+ run on-demand
+ scaling is automated

# Benefits of using Lambda

+ Pay per request and compute time (free tier is allowed 1 million AWS lambda requests and 400,000 GB of compute time)
+ Integrated well with many AWS services, number of programming languages
+ Easy monitoring using cloud watch
+ Easy to get more resources per function up to 10GB of RAM, increase in RAM also improves CPU and n/w

# PS
+ Lambda Container Image: The container image must implement Lambda Runtime API, ECS/Fargate is preferred for running arbitrary Docker images (imp for exam)

# AWS services which can be integrated with Lambda
 + **API Gateway** - used to create REST api which will invoke lambda functions
 + **Kinesis** - data transformations can be done dynamically using lambda functions
 + **Dynamo DB** - triggers can be created to invoke lambda functions
 + **S3** - to know when a file is added in S3
 + **CloudFront**
 + **Cloudwatch Events - Event Bridge**
 + **SNS**
 + **SQS**
 + **Cognito** - on login

![vlcsnap-2024-08-26-22h51m20s815](https://github.com/user-attachments/assets/1ec079ef-5fed-42f9-8532-4f1ce7e81c60)
![vlcsnap-2024-08-26-23h17m03s672](https://github.com/user-attachments/assets/9658a43c-daea-48f7-9487-9b4f63effe06)
![vlcsnap-2024-08-26-23h17m58s380](https://github.com/user-attachments/assets/7c38d0e8-3884-478e-bfb9-326275162064)

