# Module-1-Homework-Docker-SQL
Answers to Module 1 Homework DE Zoomcamp

Question 1. Version of pip

24.3.1> this one


Demostration using WSL:

root@WIN-V675S0OPII4:~/data-engineering-zoomcamp# docker run -it --entrypoint=bash python:3.12.8
root@ba39565c332b:/# pip --version
pip 24.3.1 from /usr/local/lib/python3.12/site-packages/pip (python 3.12)


Question 2. Given the following docker-compose.yaml, what is the hostname and port that pgadmin should use to connect to the postgres database?

db:5432 > this one, the hostname to connect to postgress is the same as the service defined in *.yaml, which is "db". the internal port used by postgres database is 5432.

Question 3.-Question 6. see upload_data.ipynb file SQL section.


Question 7. Terraform Workflow
Which of the following sequences, respectively, describes the workflow for:

Downloading the provider plugins and setting up backend,
Generating proposed changes and auto-executing the plan
Remove all resources managed by terraform`
Answers:

terraform import, terraform apply -y, terraform destroy
teraform init, terraform plan -auto-apply, terraform rm
terraform init, terraform run -auto-approve, terraform destroy
terraform init, terraform apply -auto-approve, terraform destroy > this one
terraform import, terraform apply -y, terraform rm


The correct answer is: terraform init, terraform apply -auto-approve, terraform destroy

terraform init: Initializes & configures the backend, installs plugins/providers, & checks out an existing configuration from a version control.
terraform apply -auto-approve: this generates a plan and applies the changes automatically without requiring interactive approval
terraform destroy: this removes all resources managed by Terraform.
