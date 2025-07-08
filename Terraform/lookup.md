## Error:

 Error: Invalid function argument
│
│   on ec2.tf line 4, in resource "aws_instance" "roboshop":
│    4:     instance_type = lookup(var.instance_type, terraform.workspace)
│     ├────────────────
│     │ while calling lookup(inputMap, key, default...)
│     │ var.instance_type is object with 2 attributes
│
│ Invalid value for "inputMap" parameter: the given object has no attribute
│ "default".
╵
Releasing state lock. This may take a few moments...


## solution:
 we must include default value 
 lookup(var.instance_type, terraform.workspace,"t3small")
