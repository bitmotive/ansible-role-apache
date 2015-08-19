ansible-role-apache
=========

Apache configuration

Requirements
------------

This role has only been tested on EL 6 systems using Ansible 1.9.

Role Variables
--------------

__apache_paths__: Directories that must be created when installing Apache. 

__apache_modules__: An array of modules to be added after Apache is installed.

__apache_vhosts_files__: The name of the Virtual Host configuration files to be copied to the server.

Example Playbook
----------------

```
- hosts: webservers
  roles:
    - { role: bitmotive.ansible-role-apache, tags: "apache" }
```

License
-------

MIT
