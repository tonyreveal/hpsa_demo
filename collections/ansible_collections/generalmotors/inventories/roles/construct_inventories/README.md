Construct Inventories
=========

Reads host information from a PostgreSQL database.  Then creates inventories and hostgroups (based on site) in Automation Platform (AAP).  The correct AAP Instance Group is associated with the inventories for the site.  Hostgroups cannot be associated with an Instance Group but an Instance Group can be selected at Runtime when launching a job.

Requirements
------------

PostgreSQL queries require the psycopg2 database adapter.

Role Variables
--------------

v1 of this role does not have any input variables.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

```yaml
---
- name: Create Inventories in AAP from database information
  hosts: localhost
  gather_facts: false
  roles:
    - role: generalmotors.inventories.construct_inventories
  
```

License
-------

MIT

Author Information
------------------

Tony Reveal (treveal@redhat.com)
