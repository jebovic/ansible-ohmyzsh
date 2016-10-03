OhMyZsh
=======

[![Build Status](https://travis-ci.org/jebovic/ansible-ohmyzsh.svg?branch=master)](https://travis-ci.org/jebovic/ansible-ohmyzsh) [![Ansible Galaxy](https://img.shields.io/badge/galaxy-jebovic.ohmyzsh-blue.svg?style=flat)](https://galaxy.ansible.com/jebovic/ohmyzsh)

Install and configure Oh My Zsh for your personal user

Requirements
------------

Need zsh to be installed first

Role Variables
--------------

```
# Choose user who you want to install oh my zsh for
ohmyzsh_for: ops
go_path: /srv/golang
```

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - { role: jebovic.ohmyzsh }
```

License
-------

MIT

Author Information
------------------

Jérémy Baumgarth https://github.com/jebovic
