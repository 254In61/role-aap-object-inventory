# role-aap-object-credential
Ansible role to build AAP workflow objects

# Ref
https://console.redhat.com/ansible/automation-hub/repo/published/ansible/controller/content/module/schedule/

# How to use

Step 1: Install the role in your environment.
  - You could have roles/requirements.yml if running on AAP.
  - Or simple install on your environment.

Step 2: Define your variables in the structure below

  - build: true/false # Bool value to switch role on off.
  - inventory: "{{ inventory_name }}"
  - inventory_source: "{{ inventory_source_name }}"
  - source_path: "{{ inventory_source_file_path }}"
  - organization: "{{ organization_name }}"
  - project: "{{ project_name }}"
  - credential: "{{ git_credential }}"
  - description: "{{ common_description }}"

Step 3: Call the role from your playbook.

# Example

## varible definition in group_vars/*.yml
example-vars.yml

NB: It is assumed you are using inventory-as-code i.e inventory is pulled from the git repository and NOT hardcoded in the AAP
  
## playbook
example-playbook.yml
