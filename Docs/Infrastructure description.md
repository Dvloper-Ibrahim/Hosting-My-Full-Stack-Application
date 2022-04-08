# Infrastructure Description
This app is hosted on Amazon WWeb Services ( AWS ) and the services that uses are :

- Elastic Beanstalk
- RDS
- S3

## RDS
RDS is a provided service from AWS to create databases. When the user is requesting to get data or to save it , RDS is the great choice to do that.

## Elastic Beanstalk
- Elastic Beanstalk is a good service to host the app's server.
- Using EB we run Udagram's server on an environment with some declared variables like ( database port , AWS_REGION , JWT_SECRET ,... ), and of course these variables are hidden from the code.

## S3
S3 is the service used to save files in AWS as well as host static website that is connected to its server side through requests.

***Look at the diagrams folder to see the relations between these services and the user.***
