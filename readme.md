Project Repository

This repository contains configuration files, scripts, and documentation for provisioning and configuring AWS infrastructure using Terraform and Ansible. The project is organized into three main directories:

    terraform_config: Contains the Terraform configuration for provisioning AWS resources, with subdirectories for different components.

    ansible_config: Contains Ansible playbooks and configuration files for configuring the provisioned AWS servers. The directory structure here mirrors that of the terraform_config directory.

    scripts: Contains various scripts to assist with managing the infrastructure and other automation tasks.

Directory Structure

    terraform_config: This directory contains subdirectories for different AWS components, including:

        jenkins: Terraform configuration for provisioning a Jenkins server.

        sonar: Terraform configuration for provisioning a SonarQube server.

        nexus: Terraform configuration for provisioning a Nexus Repository server.

        master: Terraform configuration for provisioning the master server.

        node1: Terraform configuration for provisioning a Node1 server.

    ansible_config: This directory mirrors the terraform_config directory and contains Ansible playbooks and configuration files for configuring each AWS component.

    scripts: This directory contains various scripts to assist with managing the infrastructure, including:

        access_details.sh: Script for retrieving access details to the provisioned servers.

        generate_ansible_inventory.sh: Script for generating an Ansible inventory file based on the provisioned AWS infrastructure.

        phase1.sh: Script for running the initial setup and configuration of the AWS infrastructure using Terraform and Ansible.

        playall.sh: Script for executing Ansible playbooks for all components.

        t_createall.sh: Script for creating all AWS resources using Terraform.

        t_destroyall.sh: Script for destroying all AWS resources provisioned with Terraform.

Getting Started

    Make sure you have the necessary credentials and AWS CLI configured for Terraform to work.

    Use the t_createall.sh script to provision the AWS resources using Terraform.

    Once the AWS resources are provisioned, use the generate_ansible_inventory.sh script to create an Ansible inventory file.

    Run the phase1.sh script to configure the AWS servers using Ansible.

    You can also use individual scripts or specific playbooks for each component if needed.

Cleanup

If you want to tear down the AWS resources, you can use the t_destroyall.sh script to destroy all provisioned resources.

Contact

If you have any questions or need further assistance, please contact "zerqqaouiyassine1@gmail.com".