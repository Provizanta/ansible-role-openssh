Ansible role: openssh
=========

![main Build status](https://github.com/Provizanta/ansible-role-microk8s/actions/workflows/main.yml/badge.svg)

Install and configure an OpenSSH server.

Highly inspired by:
- https://github.com/robertdebock/ansible-role-openssh

Requirements
------------

None

Role Variables
--------------

These variables are defined in [defaults/main.yml](./defaults/main.yml):

    openssh_configuration: {}

    openssh_configuration_match_blocks: {}


Dependencies
------------

None

Example Playbook
----------------

    - name: Converge
      hosts: all
      roles:
        - role: ansible-role-openssh
          vars:
            openssh_configuration:
              Port: "22"
            openssh_configuration_match_blocks:
              Address 192.168.1.*:
                PasswordAuthentication: "yes"
                PermitRootLogin: "yes"

License
-------

MIT

Author Information
------------------

Tibor Csóka
