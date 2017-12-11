Satis Ansible Role
==================

[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-HanXHX.satis-blue.svg)](https://galaxy.ansible.com/HanXHX/satis/) [![Build Status](https://travis-ci.org/HanXHX/ansible-satis.svg?branch=master)](https://travis-ci.org/HanXHX/ansible-satis)

This is an ansible role for installing satis through composer.

Requirements
------------

- php
- composer
- git

Role Variables
--------------

### System

- `satis_user`
- `satis_group`
- `satis_user_home`

### Install

- `satis_installation`: Install directory
- `satis_config_file`: Satis configuration file
- `satis_build_dir`: Build directory
- `satis_manage_cron`: (bool) manage crontab 
- `satis_version`: Satis version to install (alpha for latest pre-release, dev for master branch)

### Configuration

- `satis_repo_name`: (string) Repository name
- `satis_repo_homepage`: (string) Repository URL
- `satis_repos`: (hashlist)
- `satis_require`: null (is don't needed) or key/value hash with repositories version
- `satis_skip_dev`: (bool)
- `satis_composer_ignore_secure_http`: (bool)
- `satis_require_all`: (bool)
- `satis_require_dependencies`: (bool)
- `satis_require_dev_dependencies`: (bool)

Dependencies
------------

None.

Example Playbook
----------------

See [test playbook](tests/test.yml).

License
-------

MIT

Author Information
------------------

- Twitter: [@hanxhx_](https://twitter.com/hanxhx_)
