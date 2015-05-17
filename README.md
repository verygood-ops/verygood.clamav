Role Name
=========

This roles setup a Clamav

Requirements
------------

This role is only tested on Ubuntu trusty. ClamAV eats up about 300mb of ram.

Role Variables
--------------



Example Playbook
----------------

    - hosts: agents
      roles:
         - verygood.ossec-clamav

License
-------

BSD
