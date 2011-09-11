Description
===========

Installs and configures top.

Requirements
============

Platform:

* Debian
* Ubuntu
* CentOS
* RedHat
* Fedora

At the moment there're no dependencies to other cookbooks.

Attributes
==========

* node['top']['is_secure']    - Defines whether secure mode is enabled or not. Default is: true

Usage
=====

Add "recipe[top]" directly to a node or a role.

If you want to disable secure mode, set **is_secure** to **false** within a role:

    default_attributes(
      "top" => {
        "is_secure" => false
      }
    )
