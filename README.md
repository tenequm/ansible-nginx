ansible-nginx
=========
[![Build Status](https://travis-ci.org/1nfinitum/ansible-nginx.svg?branch=master)](https://travis-ci.org/1nfinitum/ansible-nginx)

This role installs nginx on the server, currently it works only with Ubuntu 16.04 LTS, it's just a skeleton that fits for now and I'm going to make it more flexible and useful with the time of use.

Requirements
------------

This role requires only root access for accomplishing its operations, so either run it in a playbook with a global `become: yes`, or invoke the role in your playbook like:
```
- hosts: localhost
  roles:
    - role: 1nfinitum.nginx
```

Role Variables
--------------

There are no variables for used in there for now, will add them when the role will be more complicated.

Example Playbook
----------------

```
- hosts: localhost
  become: yes
  roles:
    - { role: 1nfinitum.nginx }
```
License
-------

MIT

Author Information
------------------

This role was created in 2017 by [Mykhaylo Kolesnik](http://github.com/1nfinitum).
