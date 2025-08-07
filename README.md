# Terraform Docker Container Deployment 🚀

This project demonstrates how to provision a local **Docker container** using **Terraform** on a self-hosted Linux (RHEL 9) virtual machine.

## 🧰 Tools Used

- Terraform
- Docker
- Git
- Linux VM (RHEL 9)

## 📁 Repository

GitHub Repo: https://github.com/Hyghen/Terraform-Demo-Project

## ✅ Step-by-Step explanation of what i have done 


### 1️⃣ Initial Setup

- Installed Docker, Git, and Terraform on a fresh RHEL 9 Virtual Machine.
- Verified Docker is running and Terraform is installed.


### 2️⃣ GitHub Repository

- Created the repository: https://github.com/Hyghen/Terraform-Demo-Project
- Cloned it locally:

  -- git clone https://github.com/Hyghen/Terraform-Demo-Project.git
  -- cd Terraform-Demo-Project


3️⃣ Terraform Configuration

-- Created a main.tf file using HCL (HashiCorp Configuration Language).
-- Used Docker as the Terraform provider.

Defined:

A Docker image resource for nginx.
A Docker container that maps port 8080 to 80.


4️⃣ Terraform Execution Commands


-- terraform init        # Initialize the working directory

<img width="1166" height="432" alt="Screenshot 2025-08-07 123256" src="https://github.com/user-attachments/assets/0fb233bf-e8f7-4673-a62f-7df54f94e451" />



-- terraform plan        # See the execution plan

-- terraform apply       # Create the container


-- terraform state list  # Check created resources

<img width="792" height="110" alt="Screenshot 2025-08-07 124430" src="https://github.com/user-attachments/assets/7a087e64-5b8e-451f-a1e8-5ae49d75e8e3" />




-- terraform destroy     # Tear down infrastructure

<img width="1702" height="261" alt="Screenshot 2025-08-07 124547" src="https://github.com/user-attachments/assets/d2f382de-1ca8-44e2-bdd8-588a22637d9f" />



🌐 Test the Deployment

-- After applying the changes, accessed the container in browser:
-- http://192.168.1.8:8080


It showed the nginx welcome page, confirming successful deployment.



<img width="1116" height="393" alt="Screenshot 2025-08-07 124102" src="https://github.com/user-attachments/assets/e82ed510-3920-43bc-a98d-7afc7fbad2b7" />



💡 What I Learned

-- How to use Terraform Docker Provider.

-- Full cycle: init, plan, apply, state, and destroy.

-- Infrastructure as Code (IaC) in practice with Docker.


🔗 Author

Chitransh Jangid

Github Profile:  https://www.github.com/Hyghen
