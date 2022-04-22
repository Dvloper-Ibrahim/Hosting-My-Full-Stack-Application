# Pipeline Process
[![CircleCI](https://circleci.com/gh/ibrahimahmed289/Hosting-My-Full-Stack-Application.svg?style=svg)](https://circleci.com/gh/ibrahimahmed289/Hosting-My-Full-Stack-Application)

CircliCi is a helpful service to deploy versions of our app very fast saving alot of time in installing , building and deploying our app version ourselves.

## Orbs
CircleCi presents them to install common techniques without manual setup. Udagram uses :

-   `node: circleci/node@5.0.1`
-   `aws-cli: circleci/aws-cli@2.1.0`
-   `eb: circleci/aws-elastic-beanstalk@2.0.1`

## Jobs
### 1. deploy the backend :
- It installs backend packages, builds the express app and uses the EB CLI to deploy the build of the app.
### 2. deploy the frontend :
- It installs frontend packages, builds the angular app and uses the AWS CLI to deploy the build of the app.

## Workflows
We setup our workflow and organized the jobs to be implemented sequentially as well as on a particular branch of our repository.

***Look at the diagrams folder to see an overview of our pipeeline as a flowchart.***
