📘 **What is Ansible?**

Ansible is an open-source automation tool used for:

1.Configuration Management
2.Application Deployment
3.Provisioning Infrastructure
4.Orchestration of IT tasks

It allows you to describe your infrastructure as code, using simple YAML files called playbooks.

⚙️ **How Ansible Works**

Ansible connects to your systems (called hosts) over SSH and executes tasks remotely. It’s agentless, meaning you don’t need to install anything on the target machines.

🧠 **Key Concepts**

1.Playbook: A YAML file that defines what tasks to run on which hosts.
2.Inventory: A list of target machines (can be static or dynamic).
3.Task: A single action, like installing a package or restarting a service.
4.Role: A structured way to organize tasks, variables, templates, and files.
5.Facts: Automatic system information collected from hosts (e.g. IP, OS).
6.Module: A reusable Ansible component to perform tasks (e.g. apt, copy, user).

🚀 **Why Use Ansible?**

1.Simple syntax (YAML)
2.Agentless (no software to install on target machines)
3.Works on Linux, macOS, cloud, VMs, containers
4.Scales from one laptop to thousands of servers

🚀 **How to Run This Ansible Project**

📦 **Prerequisites**

A GitHub Codespace (Ansible installed with pip install --user ansible)

**Basic understanding of YAML**

🛠️ **Project Structure**

ansible-demo/
├── inventory          # Inventory file with target hosts (e.g., localhost)
├── playbook.yml       # Main Ansible playbook
└── vars/
    └── common.yml     # External variables file

▶️ **Steps to Run the Playbook**

1.Open Codespace Terminal
2.Use the built-in terminal in your GitHub Codespace.
3.Run the playbook

"ansible-playbook -i inventory playbook.yml"

**Expected Output**

Prints a greeting message using your system hostname
Creates a file at /tmp/hello_from_var.txt
Shows system facts (RAM, OS, interfaces, etc.)
