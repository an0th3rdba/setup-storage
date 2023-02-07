Role name: setup-storage
========================

Ansible role to prepare disks before starting any further software installation (PostgreSQL for example).

Requirements
-------------

Devices/disks to be part of the LVM setup must be attached to server prior to using this role.

There should not be any kind of partitions on disks.

Ensure that you select the correct devices/disks.

Example Playbook
----------------
```
- hosts: all
  roles:
      - { role: setup-storage, become: true }
```
License
-------

MIT
