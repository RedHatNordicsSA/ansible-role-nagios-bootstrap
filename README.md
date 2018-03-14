Role Name
=========

This role adds a server to be monitored by Nagios

Requirements
------------

The monitored client need to have prereqs in place, these are handled by the ansible-role-nagios-nrpe role.

Role Variables
--------------

monitored_server: fqdn-of-server-to-monitor

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: nagios.redhat.labrats.se
      roles:
         - ansible-role-nagios-bootstrap
      vars:
         monitored_server: "{{ short_hostname + '.' + domain }}"


License
-------

GPL 3.0

Author Information
------------------

Magnus Glantz, sudo@redhat.com, 2018