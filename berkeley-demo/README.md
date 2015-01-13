## Berkeley Demo AWS templates

### Non-cluster template

This template creates one instance of each type (client, server, kafka, cassandra, spark) in two subnets )public and private of a single VPC.

Just create the CloudFormation stack with the berkeley-demo-stack.json template and find the EIP of the command box in outputs.
Now use your SSH client of choice to connect to the Command Box with this EIP and upload your key file in the ~/.ssh folder to be able to connect the following boxes in the private subnet:

10.0.10.10 - device emulator client

10.0.10.20 - device connection server

10.0.10.30 - Kafka node

10.0.10.40 - Cassandra node

10.0.10.50 - Spark node


By default no software installed on boxes - keep updated.
