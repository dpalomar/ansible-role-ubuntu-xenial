Ubuntu.Xenial64
=========

This role allows to install Ansible on Official Canonical Ubuntu 16.04.

If you wants provision with Ansible, you don't because it use python3 by default and actual version of Ansible does not support.

So, it is mandatory to install python 2.7 before, but you don't because ansible need python available on the system. So, we are in a loop.

This role is for fresh install of Ubuntu 16.04 Xenial, and it upgrades the system for first time, reboot, wait for restart and install some basic tools making the system available for ansible provision with others roles.

Requirements
------------

None.
Use it before other roles.

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------



    - hosts: servers
      roles:
         - { role: ansible-role-ubuntu-xenial }

License
-------

BSD / MIT

Author Information
------------------

This roles was developed by David Palomar
