[![CircleCI](https://circleci.com/gh/circleci/circleci-docs.svg?style=svg)](https://app.circleci.com/pipelines/github/3to1dash/deploy-project)

# Deployment Process Project

## Links for the Back-End and the Front-End
- Back-End: http://udagram-api.eba-vgkbirxa.us-east-1.elasticbeanstalk.com
- Front-End: http://elasticbeanstalk-us-east-1-079290547713.s3-website-us-east-1.amazonaws.com

## Dependencies
You can look at the dependencies that the backend and the frontend use in [docs/dependencies.md](/docs/dependencies.md).

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```
## Pipeline
You can look at a digram for the circleci pipelines for the backend and the frontend in [docs/pipeline.md](/docs/pipeline.md).

## Infrastructure
You can look at the infrastructure of the amazon services that the backend and the frontend use in [docs/infrastructure.md](/docs/infrastructure.md).

## Screenshots
- CircleCI Environment Variables
![CircleCI Environment Variables!](/docs/circleci_env.png "CircleCI Environment Variables")

- CircleCI last passed pipeline
![CircleCI last passed pipeline!](/docs/last_pipeline_passed.png "CircleCI last passed pipeline")

- RDS (postgresql database)
![RDS!](/docs/rds.png "RDS (postgresql database)")

- Elastic Beanstalk (Back-End Application)
![AWS EB!](/docs/eb.png "Elastic Beanstalk (Back-End Application)")

- S3 (Front-End Application)
![S3!](/docs/bucket.png "S3 (Front-End Applicaion)")