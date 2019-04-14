Ansible Role: Oracle Java
=========

[![Build Status](https://travis-ci.org/webarchitect609/ansible-role-oracle-java.svg?branch=master)](https://travis-ci.org/webarchitect609/ansible-role-oracle-java)

Installs Oracle Java via ppa repository. 

Requirements
------------

None.


Role Variables
--------------
None of variables is needed to be altered for install Oracle Java 12 from [Linux Uprising PPA](https://launchpad.net/~linuxuprising/+archive/ubuntu/java).
But all available variables are listed below, along with default values (see `defaults/main.yml`):

    java_packages: "oracle-java12-installer"

Package to install Java.

    java_set_default_package: "oracle-java12-set-default"

Package to set this version of Java used by default. 

    java_set_default: true

Whether to set this version of Java to be used by default.

    java_repo: "ppa:linuxuprising/java"

PPA for Ubuntu and Linux Mint.

    java_deb_source: "deb http://ppa.launchpad.net/linuxuprising/java/ubuntu bionic main"
    java_key_server: "hkp://keyserver.ubuntu.com:80"
    java_key: "73C3DB2A"

Same parameters for Debian.
 

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: webarchitect609.oracle_java }

License
-------

MIT

Author Information
------------------

This role was created in 2019 by Gripinskiy Sergey.
