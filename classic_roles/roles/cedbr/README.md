Role Name
=========

Role name "classic_roles" - Its a classic way of using roles. This role have the below tasks for practising/testing purpose. 

This play book works fine on RHEL8, OEL8 and RHEL9.

content:
   -  user_group.yml
   -  creating_sshkey_and_passing.yml
   -  package_install.yml
   -  user_password_set.yml
   -  copying_files_to_remote_hosts.yml
   -  backingup_files_commenting_a_line.yml
   -  using_jinja2.yml

Requirements
------------

Ansible master node - 1 - Ansible installed with latest version and its subscribed to Redhat
Remote hosts - depends on your idea.

OS used: RHEL8, OEL8 and RHEL9.
RHEL systems are subscribed to Redhat

Role Variables
--------------

Yet to set valut - in progress

Dependencies
------------

As authorized_key module is not such comapatible with the latest version of ansible got error when tried to run the play. 

To ovecome this, have used collections from ansible-galaxy to collect the latest collection of "authorized_key" module.

Once its downloaded locally we need to mention this in ansible.cfg file to get the playbook work.

"COLLECTIONS_PATH = /collections"

License
-------

BSD

Author Information
------------------

https://github.com/Nathi-86/Ansible_2024
