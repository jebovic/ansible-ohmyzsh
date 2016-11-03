OhMyZsh
=======

[![Build Status](https://travis-ci.org/jebovic/ansible-ohmyzsh.svg?branch=master)](https://travis-ci.org/jebovic/ansible-ohmyzsh) [![Ansible Galaxy](https://img.shields.io/badge/galaxy-jebovic.ohmyzsh-blue.svg?style=flat)](https://galaxy.ansible.com/jebovic/ohmyzsh)

Install and configure Oh My Zsh for a list of users

This role is a part of my [OPS project](https://github.com/jebovic/ops), follow this link to see it in action. OPS provides a lot of stuff, like a vagrant file for development VMs, playbooks for roles orchestration, inventory files, examples for roles configuration, ansible configuration file, and many more.

Requirements
------------

Need zsh to be installed first

Role Variables
--------------

```yaml
# Choose user who you want to install oh my zsh for
ohmyzsh_users:
  - username: ops
    usergroup: admin
    home: /home/ops
  - username: root
    usergroup: root
    home: /root

ohmyzsh_plugins: git colored-man-page colorize extract history npm symfony2 httpie zsh-syntax-highlighting
```

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: jebovic.ohmyzsh }
```

Tags
----

* ohmyzsh_config : only update config

License
-------

MIT

Author Information
------------------

Jérémy Baumgarth https://github.com/jebovic
