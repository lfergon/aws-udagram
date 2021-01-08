# Deploy a High-Availability Web App using CloudFormation

## Chart infrastructure

   ![Chart infrastructure](https://github.com/lfergon/aws-udagram/blob/master/udagram_route_table.jpeg?raw=true)

## Deploy infrastructure

    1. ./utils/create.sh networkaws network.yml network-params.json

## Deploy JumpBox/Bastion

    2. ./utils/create.sh jumpbox-host-server jumpbox.yml jumpbox-params.json 

## Deploy Web Applications, Autoscaling Groups, LoadBalancers

    3. ./utils/create.sh serversstack servers.yml servers-params.json


