pip_venv ansible role
=====================

![CI](https://github.com/baztian/ansible-pip-venv/workflows/CI/badge.svg)

Ansible role for installing python modules inside a new virtual env inside
`/opt/<pkg-name>`. For packages like `molecule[docker]` you can overwrite
the folder name with `dir` var.

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
            extra_pkgs:
              - markupsafe==2.0.1

License
-------

MIT
