journalbeat-role
=========

Installs and configures journal beat

Role Variables
--------------
Requires the following variables to be overridden:

        journalbeat:
          field_metadata:
            team: optimus
            environment: notset
          tags: ['application']
          units: ['nginx.service']
          logstash:
            hosts: ['localhost:5200', '2:11']

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: devops.journalbeat,  }

License
-------

MIT

Author Information
------------------

HMCTS reform programme.
