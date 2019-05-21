Role Name
=========

![ansible-ntp](https://img.shields.io/github/issues/spy86/ansible-ntp.svg) ![ansible-ntp](https://img.shields.io/github/forks/spy86/ansible-ntp.svg) ![ansible-ntp](https://img.shields.io/github/stars/spy86/ansible-ntp.svg) ![ansible-ntp](https://img.shields.io/github/license/spy86/ansible-ntp.svg) ![ansible-ntp](https://img.shields.io/twitter/url/https/github.com/spy86/ansible-ntp.svg?style=social)

Role to set up [NTP-Service](http://www.pool.ntp.org/)


Requirements
------------

None

Role Variables
--------------

- `ntp_servers` - List of NTP servers to be used for time syncronization.

Dependencies
------------

None

Example Playbook
----------------

```YAML
---
- hosts: servers
  remote_user: root
  roles:
   - role: ansible-ntp
     vars:
        ntp_servers:
          - 0.it.pool.ntp.org
          - 1.it.pool.ntp.org
          - 2.it.pool.ntp.org
          - 3.it.pool.ntp.org

```
