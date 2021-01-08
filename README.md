# Deploy a High-Availability Web App using CloudFormation

## What to implement

   Your company is creating an Instagram clone called Udagram. Developers pushed the latest version of their code in a zip file located in a public S3 Bucket.

   Deploy the application, along with the necessary supporting software into its matching infrastructure.

   This needs to be done in an automated fashion so that the infrastructure can be discarded as soon as the testing team finishes their tests and gathers their results.


## Chart infrastructure

   ![Chart infrastructure](https://github.com/lfergon/aws-udagram/blob/master/udagram_route_table.jpeg?raw=true)

## Deploy infrastructure

    1. ./utils/create.sh networkaws network.yml network-params.json

## Deploy JumpBox/Bastion

    2. ./utils/create.sh jumpbox-host-server jumpbox.yml jumpbox-params.json 

## Deploy Web Applications, Autoscaling Groups, LoadBalancers

    3. ./utils/create.sh serversstack servers.yml servers-params.json


