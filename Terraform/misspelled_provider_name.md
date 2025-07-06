## ERROR:

DELL@DESKTOP-LNC7QP1 MINGW64 ~/Documents/AWSDEVOPS/repo/terraform
$ terraform init
Initializing the backend...
Initializing provider plugins...
- Finding hashicrop/aws versions matching "5.98.0"...
╷
│ Error: Failed to query available provider packages
│
│ Could not retrieve the list of available versions for provider
│ hashicrop/aws: provider registry registry.terraform.io does not have a
│ provider named registry.terraform.io/hashicrop/aws
│
│ All modules should specify their required_providers so that external
│ consumers will get the correct providers when using a module. To see which
│ modules are currently depending on hashicrop/aws, run the following
│ command:
│     terraform providers

## SOLUTIONS:

i mis spelled name hashicorp to hashicrop:
