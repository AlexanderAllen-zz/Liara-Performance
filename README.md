Liara/Performance
=============

Ansible role for improving performance on virtual LAMP stacks.

Requirements
------------

- PHP
- Liara

Role Variables
--------------

This role uses the `liara_performance_environment` variable to determine which performance
settings to load.

Dependencies
------------

This role depends on `AlexanderAllen.Liara` for the `liara_php_mod_dir` and `liara_php_conf_dir`
PHP configuration variables.

Example Playbook
----------------

    - hosts: webservers
      roles:
         - { role: AlexanderAllen.Liara-Performance }

Inside `vars/main.yml`:

    ---
    # Used to determine what performance settings to load, example: [local|dev|qa|prod]
    liara_performance_environment: "local"

License
-------

GPLv2

Author Information
------------------

https://github.com/AlexanderAllen
