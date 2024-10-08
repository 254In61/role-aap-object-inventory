# role-aap-object-credential
Ansible role to build AAP workflow objects

# Ref
https://console.redhat.com/ansible/automation-hub/repo/published/ansible/controller/content/module/schedule/

# How to use

Step 1: Install the role in your environment.
  - You could have roles/requirements.yml if running on AAP.
  - Or simple install on your environment.

Step 2: Define your variables. See example-vars.yml

Step 3: Call the role from your playbook. See example-playbook.yml

# Example

## varible definition in group_vars/*.yml
example-vars.yml

NB: It is assumed you are using inventory-as-code i.e inventory is pulled from the git repository and NOT hardcoded in the AAP
  
## playbook
example-playbook.yml
