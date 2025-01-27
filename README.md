# Module-1-Homework-Docker-SQL
Answers to Module 1 Homework DE Zoomcamp

Question 1. Version of pip

24.3.1> this one
24.2.1
23.3.1
23.2.1

Demostration using WSL:

root@WIN-V675S0OPII4:~/data-engineering-zoomcamp# docker run -it --entrypoint=bash python:3.12.8
root@ba39565c332b:/# pip --version
pip 24.3.1 from /usr/local/lib/python3.12/site-packages/pip (python 3.12)


Question 2. Given the following docker-compose.yaml, what is the hostname and port that pgadmin should use to connect to the postgres database?

postgres:5433
localhost:5432
db:5433
postgres:5432
db:5432 > this one, the hostname to connect to postgress is the same as the service defined in *.yaml, which is "db". the internal port used by postgres database is 5432.

Question 3.-Question 6. see upload_data.ipynb file.

Question 7.
The correct answer is: terraform init, terraform apply -auto-approve, terraform destroy

Explanation of the correct sequence:
terraform init: Initializes & configures the backend, installs plugins/providers, & checks out an existing configuration from a version control.
terraform apply -auto-approve: this generates a plan and applies the changes automatically without requiring interactive approval
terraform destroy: this removes all resources managed by Terraform.
