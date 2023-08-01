wp_install
==========

Installs Wordpress on your host.

This role is meant for simple deployments where web and database server run on the same host. The database for the Wordpress instance will be created by this role.

Requirements
------------

Before using this role to install Wordpress, make sure your host meet the requirements on the server side:

  * PHP 7.4 or greater
  * MySQL 5.7 or MariaDB 10.4 or greater
  * HTTPS support

For additional information on requirements please refer to:

  * [https://wordpress.org/about/requirements/](https://wordpress.org/about/requirements/)
  * [https://make.wordpress.org/hosting/handbook/server-environment/](https://make.wordpress.org/hosting/handbook/server-environment/)

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Before this role can be used it is mandatory to define the following variables from `defaults/main.yml`:

~~~
wp_db_name:     # Database name
wp_db_user:     # Name of the database user for Wordpress
wp_db_pass:     # Password for the database user
wp_web_root:    # Absolute path the document root directory
~~~

The variables in `defaults/main.yml` are left blank intentionally, because for this role it's better to fail early than causing serious damage to the system.

Variables from `vars/Debian.yml` to make sure necessary packages are installed:

~~~
wp_packages:
  - python3-mysqldb
  - python3-pymysql
  - mariadb-client
~~~

Dependencies
------------

To use this role the collection `community.mysql` needs to be installed.

Example Playbook
----------------

**Follows after testing!**

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

  * Joerg Kastning <joerg(dot)kastning(aet)my-it-brain(dot)de>
  * Website: https://www.my-it-brain.de
