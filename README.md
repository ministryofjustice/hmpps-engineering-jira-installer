jira-install
=========

Ansible role to install a given version of JIRA Server.
This role is primarily designed to install v6.x of JIRA as part of the AWS migration of nDelius and supporting systems.

Requirements
------------

 - botocore
 - boto
 - boto3

Role Variables
--------------

 - jira_user: JIRA user (default = jira)
 - jira_group: Group for JIRA user (default = jira)
 - jira_user_home_dir: JIRA User and Install Dir (default = /home/jira"
 - jira_home: JIRA Data Dir (default = /var/jira)
 - jira_filename: JIRA Install Artefact File name prefix (fefault = atlassian-jira)
 - jira_version: JIRA Veriosn (default = 6.4.9)
 - jira_artefact_bucket: S3 Artefact Bucket for JIRA Install Files (default = tf-eu-west-2-hmpps-eng-dev-artefacts-s3bucket)

Dependencies
------------

 - botocore
 - boto3

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
