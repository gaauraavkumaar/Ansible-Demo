# 🚀 Ansible Demo: Docker + NGINX on GCP VM

## ✅ Steps Performed

1. Created a VPC named `gaurav-vpc`
2. Created a subnet named `gaurav-subnet` under the VPC
3. Created a VM named `gaurav-ansible-vm` inside the subnet using GCP CLI
4. Verified that Python3 is pre-installed on the VM
5. Installed Ansible on my local machine (Mac)
6. Created an `inventory.ini` file with the VM’s external IP and SSH details
7. Wrote an Ansible playbook (`setup.yml`) to:
   - Install Docker on the VM
   - Run an NGINX container on port 80
8. Allowed HTTP (80) and SSH (22) traffic using firewall rules
9. Ran the Ansible playbook from my local machine using:
   ```bash
   ansible-playbook -i inventory.ini setup.yml
10.	Verified that the NGINX container is running on the VM
11.	Accessed the NGINX welcome page via the VM’s external IP in the browser
12.	Pushed the Ansible project to this GitHub repository