Ansible role: openssh
=========

[![Build Status](https://travis-ci.com/Provizanta/ansible-role-openssh.svg?branch=main)](https://travis-ci.com/Provizanta/ansible-role-openssh)

Install openssh server configuration.

Requirements
------------

None

Role Variables
--------------

These variables are defined in [defaults/main.yml](./defaults/main.yml):


These variables do not have a default value and can be specified:

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: openssh
          vars:

License
-------

MIT

Author Information
------------------

Tibor Csóka
