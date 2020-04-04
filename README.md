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
             pkg: small
             version: 0.1.0

License
-------

MIT
