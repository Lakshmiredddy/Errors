## Problem:

aws_security_group.allow_all: Creating...
aws_security_group.allow_all: Creation complete after 7s [id=sg-075f00630009aea9a]
aws_instance.roboshop: Creating...
╷
│ Error: creating EC2 Instance: operation error EC2: RunInstances, https response error StatusCode: 400, RequestID: da14fd7b-1222-41a8-8d67-d598d08ee4c3, api error InvalidParameterValue: Value () for parameter groupId is invalid. The value cannot be empty
│
│   with aws_instance.roboshop,
│   on ec2.tf line 1, in resource "aws_instance" "roboshop":
│    1: resource "aws_instance" "roboshop" {

## solution:

security_groups -----> vpc_security_group_ids
