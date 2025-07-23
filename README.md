Terraform Module to provision an AWS EC2 instance with the latest Amazon Linux 2023 ami and install Docker on it.

Not intended for production use. It is an example module.

It is just for showing how to create a publish module in the Terraform Registry.

Usage:

```hcl

provider "aws" {
  region = "us-east-1"
}

module "docker_instance" {
    source = "Nur-Betul33/docker-instance/aws"
    key_name = "nur"
}
```