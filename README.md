#  DevOps Task : Infrastructure as Code (IaC) with Terraform

##  Objective
Provision a local **Docker container** using **Terraform**, demonstrating Infrastructure as Code (IaC) principles.

---

##  Tools & Technologies Used

- [Terraform](https://www.terraform.io/)
- [Docker](https://www.docker.com/)
- Terraform Docker Provider

---

##  Files in This Repo
 
 File                                      Description 
 `main.tf`                                 Terraform configuration to create a Docker container 
 `.terraform.lock.hcl`                     Terraform provider lock file 
 `terraform.tfstate`                       State file tracking current infrastructure 
 `terraform.tfstate.backup`                Backup of the previous state 
 `terraform.exe`                           Terraform executable (Windows) 
 `LICENSE.txt`  License information 
 `README.md`  Project explanation and workflow (you are here!) 

---

##  Prerequisites

- Docker must be installed and running locally
- Terraform must be available (included as `terraform.exe` in this repo or install separately)
- Windows OS (if using `terraform.exe` provided)

---

##  Step-by-Step Workflow

 1️. Initialize Terraform 

```bash
terraform init
```bash 

 ## 2. Preview the Plan

```bash
terraform plan

Shows what changes will be made without applying them (safe to check before applying).

 3. Apply the Configuration
```bash
terraform apply

Provisions a Docker container using the configuration in main.tf.
We will be prompted with:
Do you want to perform these actions?
Type yes and press Enter.

 4. Terraform will then proceed to:
Pull the Nginx Docker image (if not already pulled)
Create the Docker container
Map port 8888 → 80

 5. It will work on

```bash
http://localhost:8888


