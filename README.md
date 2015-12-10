NFS Server Ansible role
=======================

Installs and configures a NFS server.

Role Variables
--------------

    nfs_server_exports:
      - dir:
        allow:
        options:  # optional

    nfs_server_default_options

Example Playbook
----------------

    - hosts: localhost
      roles:
         - role: nfs_server
           nfs_server_exports:
             - dir: /srv/nfs
               allow: 192.168.0/24

License
-------

MIT
