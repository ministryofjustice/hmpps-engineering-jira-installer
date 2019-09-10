hmpps-engineering-jira-installer
=========

Ansible role to install a given version of JIRA Server.
This role is primarily designed to support v6.x of JIRA as part of the AWS migration of nDelius and supporting systems.

Requirements
------------

 - botocore
 - boto
 - boto3

Role Variables
--------------



Dependencies
------------

None

Example Playbook
----------------

---
- hosts: localhost
  roles:
    - jira-install

License
-------

MIT

Author Information
------------------
HMPPS Digital Studio
