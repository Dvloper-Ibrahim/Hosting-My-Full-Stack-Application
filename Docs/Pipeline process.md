# Pipeline Process
CircliCi is a helpful service to deploy versions of our app very fast saving alot of time in installing , building and deploying our app version ourselves.

## Orbs
CircleCi presents them to install common techniques without manual setup. Udagram uses :

-   node: circleci/node@5.0.1
-   aws-cli: circleci/aws-cli@2.1.0
-   eb: circleci/aws-elastic-beanstalk@2.0.1

## Jobs
### 1. build :
- It installs node packages and creates the build folder `( www folder )` for the express and angular apps.
### 2. deploy the backend :
- It installs node packages and uses the EB CLI to deploy the build of express app.
### 3. deploy the frontend :
- It installs node packages and uses the AWS CLI to deploy the build of angular app.

## Workflows
We setup our workflow and organized the jobs to be implemented sequentially as well as on a particular branch of our repository.

***Look at the diagrams folder to see an overview of our pipeeline as a flowchart.***
