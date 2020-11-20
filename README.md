pip_venv ansible role
=====================

![CI](https://github.com/baztian/ansible-pip-venv/workflows/CI/badge.svg)

Ansible role for installing python modules inside a new virtual env.

Example Playbook
----------------

    - hosts: servers
      become: yes
      roles:
         - role: baztian.pip_venv
           vars:
             pkg: bump2version
             version: 1.0.1
             system_site_packages: yes


License
-------

MIT
