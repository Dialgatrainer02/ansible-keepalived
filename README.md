Role Name
=========

installs keepalived and a very simple config to tracka process and failover if it dies

Requirements
------------

running rhel based distro

Role Variables
--------------

keepalived_key the password used to attach instances together
keepalived_vip the virtual ip keepalived will use
keepalived_track_process the process name to track in keepalived
keepalived_state sets the keepalived state for the host (defaults to backup)

Dependencies
------------

all self contained

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - keepalived
           vars:
             keepalived_vip: 10.0.2.200
             keepalived_track_process: sshd
             keepalived_key: 12345

License
-------

BSD

Author Information
------------------

olivia barker
