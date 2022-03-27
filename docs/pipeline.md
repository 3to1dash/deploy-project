This Project uses CircleCI pipeline to build and deploy this application to the AWS services. You can find the pipeline config file in [.circleci/config.yml](/.circleci/config.yml).

# Pipeline Layout

## Orbs
This pipeline uses three different orbs to install the needed dependencies which are:

- circleci/node@5.0.1
- circleci/aws-cli@2.1.0
- circleci/aws-elastic-beanstalk@2.0.1

## Jobs
There are Two main jobs in this pipeline the first one is for installing dependencies and building the back-end and the front-end

### Build Job Steps
1. `Front-End Install`: Installing the front-end dependencies.
2. `Back-End Install`: Installing the back-end dependencies.
3. `Front-End Build`: For building the front-end angular application.
4. `Back-End Build`: For building the back-end Node API application. 
5. The last step for perserving the built application across the build and deploy jobs.

### Deploy Job Steps
1. `Back-End Elastic Beanstack initialization`: For Initialize the Elastic Beanstack environment.
2. `Back-End Deploy`: Deploy the back-end application to AWS EB service.
3. `Front-End Deploy`: Deploy the front-end application to an AWS Bucket. 

## Workflows
There is one workflow that instruct the pipeline to run deploy after the build job if successed.

- `build-approval-deploy`: requires build to successed for the deploy job to run.

## Pipeline Diagram
![CircleCI pipeline!](/docs/pipeline.png "Pipeline Diagram")