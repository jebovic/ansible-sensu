Sensu
=====

[![Build Status](https://travis-ci.org/jebovic/ansible-sensu.svg?branch=master)](https://travis-ci.org/jebovic/ansible-sensu) [![Ansible Galaxy](https://img.shields.io/badge/galaxy-jebovic.sensu-blue.svg?style=flat)](https://galaxy.ansible.com/jebovic/sensu)

Install and configure Sensu (open source version, including uchiwa)

This role is a part of my [OPS project](https://github.com/jebovic/ops), follow this link to see it in action. OPS provides a lot of stuff, like a vagrant file for development VMs, playbooks for roles orchestration, inventory files, examples for roles configuration, ansible configuration file, and many more.

Dependencies
------------

This role depends on [jebovic.redis](https://github.com/jebovic/ansible-redis) and [jebovic.rabbitmq](https://github.com/jebovic/ansible-rabbitmq) roles to be fully functional

Role Variables
--------------

```yaml
```

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: jebovic.sensu }
```

Example : config
----------------

```yaml
```

Tags
----

* sensu_config : only update config and restart service

Add slack notifications
-----------------------

```
travis encrypt "jebovic:TRAVIS_TOKEN" --add notifications.slack
```

License
-------

MIT

Author Information
------------------

Jérémy Baumgarth https://github.com/jebovic
