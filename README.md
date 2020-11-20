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
             pkg: sampleproject
             version: 2.0.0
             system_site_packages: yes
             bin: # don't link any binaries


License
-------

MIT
