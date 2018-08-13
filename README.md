spamassassin
============

[![Build Status](https://travis-ci.org/robertdebock/ansible-role-spamassassin.svg?branch=master)](https://travis-ci.org/robertdebock/ansible-role-spamassassin)

Provides Spamassassin for your system.

Context
-------
This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://robertdebock.nl/) for further information.

Here is an overview of related roles:
![dependencies](https://raw.githubusercontent.com/robertdebock/drawings/artifacts/spamassassin.png "Dependency")

Requirements
------------

Access to a repository containing packages, likely on the internet.

Role Variables
--------------

See defaults/main.yml:

- spamassassin_group: The group to run under.
- spamassassin_user: The user to run under.


Dependencies
------------

- [robertdebock.bootstrap](https://travis-ci.org/robertdebock/ansible-role-bootstrap)
- [robertdebock.rsyslog](https://travis-ci.org/robertdebock/ansible-role-rsyslog)

Download the dependencies by issuing this command:
```
ansible-galaxy install --role-file requirements.yml
```

Compatibility
-------------

This role has been tested against the following distributions and Ansible version:

|distribution|ansible 2.4|ansible 2.5|ansible 2.6|
|------------|-----------|-----------|-----------|
|alpine-edge|yes|yes|yes|
|alpine-latest|yes|yes|yes|
|archlinux|no|no|no|
|centos-6|yes|yes|yes|
|centos-latest|yes|yes|yes|
|debian-latest|yes|yes|yes|
|debian-stable|yes|yes|yes|
|fedora-latest|yes|yes|yes|
|fedora-rawhide|yes|yes|yes|
|opensuse-leap|yes|yes|yes|
|opensuse-tumbleweed|yes|yes|yes|
|ubuntu-artful|yes|yes|yes|
|ubuntu-latest|yes|yes|yes|

Example Playbook
----------------

```
- hosts: servers

  roles:
    - role: robertdebock.bootstrap
    - role: robertdebock.rsyslog
    - role: robertdebock.spamassassin
```

Install this role using `galaxy install robertdebock.spamassassin`.

License
-------

Apache License, Version 2.0

Author Information
------------------

[Robert de Bock](https://robertdebock.nl/) <robert@meinit.nl>
