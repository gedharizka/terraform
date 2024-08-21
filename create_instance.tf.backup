provider "aws" {
    region = "ap-southeast-1"
}

resource "aws_instance" "terraform_instance" {
    ami="ami-0497a974f8d5dcef8"
    instance_type="t2.micro"
    availability_zone="ap-southeast-1a"
    key_name="sg-vm"
    vpc_security_group_ids=["sg-094f41e0f11affb6c"]
    count = 1
    tags={
        Name="Instance_Terraform"
    }
}