[![Build Status](https://travis-ci.org/CSCfi/ansible-role-mariadb.svg?branch=master)](https://travis-ci.org/CSCfi/ansible-role-mariadb)

Ansible-Role: MariaDB
=========

An role which install MariaDB on RedHat/Debian servers.

Requirements
------------

None. Purpose of this role is to perform base installation with default hardenings.

Role Variables
--------------

See defaults/main.yml for the variables you can overwrite via role call as a parameter.

* mariadb_root_password: THIS_MUST_BE_SET
* mariadb_state: latest

Dependencies
------------

None

Example Playbook
----------------

    - hosts: all
      roles:
        - { role: CSCfi.mariadb, mariadb_root_password: testpass }
