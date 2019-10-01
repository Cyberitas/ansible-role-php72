Ansible Role: PHP 72
=========

Ansible role to install PHP version 7.2 on RHEL/CentOS

Requirements
------------

None.

Role Variables
--------------

Additional php extensions are installled when passed in as list items in group_vars and host_vars.
The php_packages_additional takes a list of php extensions to be added in all environments.
```$xslt
php_packages_additional:
  - php-pecl-memcache
```

The php_packages-devel variable takes a list of php extensions to be installed in the development environment.
```$xslt
php_packages_devel:
  - php-devel
```

Other optional variables include a version number.
```$xslt
web_language_role_version: "7.2"
```

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: jhd3.ansible_role_php72 }

License
-------

MIT

Author Information
------------------

Create in 2019 by James Dugger for Cyberitas Technologies, LLC
