# CloudFormation templates for static website

AWS CloudFormation templates that spawn:
* VPC with public and private subnets
* LB, AutoScaling Group
* Configures Web instances with docker container that runs apache and hosts static website

# Quickstart

To spawn up resources:
* Specify your key pair in _servers_params.json_
* Navigate to root folder of the project and run the following commands:
```shell
$ ./create.sh udagram-network network.yml network_params.json
```

Execute the following command only after the network stack is created.
```shell
$ ./create.sh udagram-servers servers.yml servers_params.json
```
