## What is this?

CloudFormation code that will create a VPC with two AZs and an IGW.
Each AZ has a public and private subnet.
Each subnet is associated with a routing table.
Private subnets reach the internet via NAT gateway.

### How to run it.

1. use `aws configure` to get creds into the AWS CLI.
2. use the scripts `create.sh` and `update.sh` to create or update stacks. Example below. It works the same for `update.sh`.

```./create.sh <my_stack_name> network.yaml params.json```

### NOTE

**Delete the stack when finished, as NAT gateways will slowly rack up charges!**


### Other Minor Notice

This was copied directly from the Udacity examples.