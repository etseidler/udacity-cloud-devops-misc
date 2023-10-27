## What is this?

CloudFormation code that will create the following:
- load balancer
- autoscaling group of EC2 servers
- security group used for auto-scaling group
- security group used for load balancer

### How to run it.

1. use `aws configure` to get creds into the AWS CLI.
2. use the scripts `create.sh` and `update.sh` to create or update stacks. Example below. It works the same for `update.sh`.

```./create.sh <my_stack_name> network.yaml params.json```

### Prerequisite

**Make sure you have created the network (from section 1 of the course, "networking" folder), before trying to create the servers and security groups.

### NOTE

**Delete the stack when finished, since long-running servers MAY incur costs**


### Other Minor Notice

This was copied directly from the Udacity examples.