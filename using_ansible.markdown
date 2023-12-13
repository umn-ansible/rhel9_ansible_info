---
layout: page
title: Using RHEl9 and Ansible
permalink: /using_ansible_and_rhel9
---

# Using RHEL9 and Ansible at the University of Minnesota

Basic operations:

1. Request a Redhat 9 virtual machine
2. If this is a public IP machine, put in a ticket to have the firewall opened for HTTP and HTTPS (and any other ports you need)
3. If you're not already using Ansible Tower, get on-boarded
4. If you need databases, request them now
5. If you need a custom DNS name, request it now
6. If you aren't already using Azure Key Vault, get on-boarded
7. Fork the UMN Sample Playbook (or start your own new Ansible playbook repo)
8. Update the inventory to point to your new host
9. Rename the playbook, group vars and host vars to match your new host
10. Configure the Ansible playbook as needed
11. Push your playbook to GitHub
12. Create a new project in Tower, point to your GitHub repo
13. Add a new inventory in Tower, point to your inventory file
14. Create a new template in Tower, point to your playbook
15. Create new secrets in tower, with your Azure identity info
16. Run your template as a job
17. Hooray!