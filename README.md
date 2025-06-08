
# DevOps Internship Task 3: Infrastructure as Code with Terraform

This repository contains the solution for provisioning a Docker container (Nginx) using **Terraform** on an AWS **t2.micro** Ubuntu instance.

---

## Task Overview

Provision a local **Docker container** using **Terraform** on a provisioned AWS EC2 instance.

---

## Tools Used

- Terraform
- Docker
- AWS EC2 (Ubuntu)
- Bash/CLI

---

## Deliverables

   main.tf
   execution logs.

##  Steps Performed

1. Launched a t2.micro EC2 Ubuntu instance on AWS.
2. Installed Docker and Terraform on the instance.
3. Wrote a `main.tf` file to define Docker provider and Nginx container.
4. Ran Terraform commands:
   ```bash
   terraform init       # initialize the project
   terraform plan       # review the execution plan
   terraform apply      # provision the infrastructure
   terraform state list # list managed resources
   terraform destroy    # destroy provisioned resources

## Files 

.main.tf: Terraform configuration file.
.init.log: Terraform initialization log.
.plan.log: Terraform plan log.
.apply.log: Terraform apply log.
.state.log: Terraform state list log.
.destroy.log: Terraform destroy log.

--
