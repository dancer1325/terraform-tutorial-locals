# Learn Terraform locals

This repo is a companion repo to the [Learn Terraform locals](https://developer.hashicorp.com/terraform/tutorials/configuration-language/locals) tutorial.

# Goal
* Use local values 
  * rather than hard-coding values 

# Prerequisites
* Terraform v1.2+
* [AWS CLI installed locally](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
* AWS account with [associated credentials](https://registry.terraform.io/providers/hashicorp/aws/latest/docs#authentication-and-configuration)

# How to run?
* `terraform init`
* `terraform apply`
  * Problems:
    * Problem1: NO result got
      * Solution: Update aws.versions
    * Problem2: module "elb_http" $ ""aws_instance" "app"" security_groups = [module.lb_security_group.this_security_group_id]
      * Solution: Switch to existing property
* `terraform destroy`
  * clean up the infrastructure

# Notes
* Order of the resources definition in Terraform configuration does NOT affect