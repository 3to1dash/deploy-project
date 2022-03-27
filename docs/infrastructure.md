# Infrastructure
This project uses three AWS services to deploy the back-end and the front-end to the cloud and also to set up and run a postgresql database.

## RDS
This is the postgresql database that runs on cloud for the back-end to save and query data from.

## Elastic BeanStalk
This is where the back-end application in running on an environment.

## S3 Bucket
S3 bucket for deploying the front-end angular application on and the bucket that Elastic Beanstalk uses to deploy the back-end.

## Infrastructure Diagram
![AWS services diagram!](/docs/infra.png "Amazon cloud services diagram")