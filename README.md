## Description:

Install Apache on a private AWS instance within an internal network using Terraform. This is achieved by utilizing a Network Address Translator (NAT) and an Elastic IP assigned to the public bastion server that acts as a secure gateway to the internal network via SSH.

-----------------------------------------
## Dependencies:

- Configure AWS locally by installing AWS CLI, and provide a programmatic IAM user with administrator permissions in the default profile.
- Install Terraform, and add it to PATH.

-----------------------------------------
## Getting Started:

- clone repository, and move to it.
```
git clone https://github.com/eslamkhaled560/terraform-aws-bastion-server.git
cd terraform-aws-bastion-server
```

- Start project, terraform install necessary dependencies
```
terraform init
```

- Check what will be created 
```
terraform plan
```

- Create the AWS infrastructure
```
terraform apply               # type yes when prompts
```

- Created two instances with Apache installed on them, you can access it with the public IP address that appears as a terraform output
-----------------------------------------
