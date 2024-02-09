Role Name
=========

Role name is "admintasks"

- creating multiple groups/users using loop module
- adding user to group
- setting password for multiple users using loop

Requirements
------------

Ansible master node and few remote nodes.

OS used: RHEL8, OEL8 and RHEL9.
RHEL systems are subscribed to Redhat

Role Variables
--------------

- ".val_pass" under vars
- creation_user_grp.yml - secured with ansible-vault by using lable for vault password (vault_identity_list = creation@vars/.val_pass)
- user_details.yml - variables used in play

Dependencies
------------

No dependencies


License
-------

BSD

Author Information
------------------
 https://github.com/Nathi-86/Ansible_2024
 
