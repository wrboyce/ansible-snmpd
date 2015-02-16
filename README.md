snmpd
=====

[![Build Status](https://travis-ci.org/wrboyce/ansible-snmpd.png)](https://travis-ci.org/wrboyce/ansible-snmpd)

Configure snmpd on Debian/Ubuntu based systems.

Role Variables
--------------

The variables `snmpd_secret` and `snmpd_cidr` are used to build the rocommunity setting.
`snmpd_location` and `snmpd_contact` can be used to set sysLocation and sysContact respectively.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: wrboyce.snmpd
           snmpd_secret: public
           snmpd_cidr: 192.168.42.42/32
           snmpd_location: Unknown
           snmpd_contact: Root <root@localhost>

License
-------

BSD

Author Information
------------------

* Will Boyce
