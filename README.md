# syslog-ng-role
Ansible Syslog-ng role for Centos 7

A simple role which installs syslog-ng and takes a set of variables from default/main.yml and pushes to a host.

Use in a play like this
```
- hosts: all
  gather_facts: yes
  remote_user: my_user_name
  become: true
  become_user: root

  roles:
    - syslog-ng-role
```
    
References:

[https://galaxy.ansible.com/slgevens/syslog-ng/](https://galaxy.ansible.com/slgevens/syslog-ng/)

[https://galaxy.ansible.com/ihrwein/syslog-ng/](https://galaxy.ansible.com/ihrwein/syslog-ng/)  
  
I took inspiration from the above roles, and made a more specific template.
