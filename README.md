ansible_role_backupPC_server
=========


[![CI](https://github.com/habbis/ansible_role_backupPC_server/workflows/CI/badge.svg)](https://github.com/habbis/ansible_role_backupPC_server/actions?query=workflow%3ACI)


This role setup backupPC server a open source backup software.

Example site.yml

```
---
- name: setup puppet agent
  gather_facts: yes
  remote_user: root
  #remote_user: ansible
  #become: yes
  #become_method: sudo
  hosts: test
  #hosts: puppet-clients
  #hosts: all
  vars_files:
    -  defaults/main.yml
    #-  defaults/secrets.yml

  roles:
    - { role: ../ansible_role_backupPC_server }
```
