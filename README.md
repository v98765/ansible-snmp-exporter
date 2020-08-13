Ansible Role: snmp_exporter
=========

Deploy and configure prometheus snmp_exporter

Requirements
------------

Ansible

Role Variables
--------------

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `snmp_exporter_version` | 0.18.0 | SNMP exporter package version |
| `snmp_exporter_web_listen_address` | "0.0.0.0:9116" | Address on which SNMP exporter will be listening |
| `snmp_exporter_auth_cp` | public | snmp community for cp molule |

Example Playbook
----------------

```text
---
- hosts: vmagent
  connection: ssh
  become: yes
  roles: 
    - ansible-snmp-exporter
```


License
-------

MIT
