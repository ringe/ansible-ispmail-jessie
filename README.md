# ISPmail Jessie Ansible Playbook #

This repository contains a playbook and roles that you can use to set up your own Debian-based mail server. Please follow the instructions at https://workaround.org/ispmail/jessie/ansible

This repository is a clone of https://git.workaround.org/chaas/ansible-ispmail-jessie.git

# Requirements #

- Vagrant (for testing) and VirtualBox
- [Ansible](https://ansible.com)
- SSH keys authentication to root@your-new-mailserver.com
- Note that you may need more memory to apply the playbook
  than you need to run the services later. Activate swap if 
  necessary.

# Usage #

1. Clone this repository
2. Install Ansible
3. Install dependencies: ```ansible-galaxy install -r requirements.yml```
4. Copy ```group_vars/all.example``` to ```group_vars/all```
5. Change parameters in group vars and hosts file
6. ```ansible-playbook ispmail.yml```

# ISPmail on Rails #

The difference from @Signum's respository is the addition of ringe/ispmail-on-rails installation and use of Let's encrypt for SSL.

# License #

Everything in this repository can be freely used under the terms of the MIT license.
