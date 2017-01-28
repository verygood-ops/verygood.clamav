Role Name
=========

This role sets up Clamav. It uses the two clamav daemons for scanning and keeping the definitions up to date.
Because clamav-daemon will not start without a definition database ready, and we don't want to wait for it
to download one, it's included in the role and copied over.

Requirements
------------

This role is only tested on Ubuntu trusty. ClamAV eats up about 300mb of ram.

Role Variables
--------------

Defaults are shown below

```yml
clamav_logsyslog: no
clamav_selfcheck: 3600
```

Example Playbook
----------------

    - hosts: agents
      roles:
         - verygood.ossec-clamav

License
-------

BSD
