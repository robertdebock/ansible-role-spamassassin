spamassassin
=========

[![Build Status](https://travis-ci.org/robertdebock/ansible-role-spamassassin.svg?branch=master)](https://travis-ci.org/robertdebock/ansible-role-spamassassin)

Provides Postfix for your system.

Requirements
------------

Access to a repository containing packages, likely on the internet.

Role Variables
--------------

See defaults/main.yml

Dependencies
------------

- robertdebock.bootstrap

Download the dependencies by issuing this command:
```
ansible-galaxy install --role-file requirements.yml
```

Example Playbook
----------------

```
- hosts: servers

  roles:
    - role: robertdebock.spamassassin
```

Install this role using `galaxy install robertdebock.spamassassin`.

License
-------

Apache License, Version 2.0

Author Information
------------------

Robert de Bock <robert@meinit.nl>
