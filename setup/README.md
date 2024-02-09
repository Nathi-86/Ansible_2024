Role Name
=========

Role name "setup" - Basic setting up of user password and copying sshkey to remote host.

Requirements
------------

Ansible master node - 1 - Ansible installed with latest version and its subscribed to Redhat
Remote hosts - depends on your idea.

OS used: RHEL8, OEL8 and RHEL9.

Role Variables
--------------

mg-pas.yml - have all the valiables which used in this play and its secured with ansible-vault and valut password is placed under vars as ".all-pass".

And the parameter used is "vault_password_file = ./vars/.all-pass"

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

