README #

### What is this repository for? ###

This repository contains Ansible Playbooks for creating and managing Environments suitable to run components like API, Accounts etc via a SHELL SCRIPT.

### How do I get set up? ###
1. Install oci-cli and configure user creds

2. Install Ansible (Install ansible version > 2.1, since few parameters from greater versions have been used in the playbooks)

3. Run the shell script as given in the next section.


### How to execute the playbooks to install various services on remote hosts? ###

As a wrapper, we have a shell script which will take component, environment, service and tag as parameters and run the playbook internally

For example:

./run-playbook.sh -c mariadb -e dr -t install,configure


