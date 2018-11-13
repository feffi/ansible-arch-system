# ansible-system

Ansible role to maintain various general system settings.

[![Build Status](https://img.shields.io/travis/feffi/ansible-system.svg)](https://travis-ci.org/feffi/ansible-system) [![Github All Releases](https://img.shields.io/github/downloads/feffi/ansible-system/total.svg)](https://github.com/feffi/ansible-system) [![GitHub forks](https://img.shields.io/github/forks/feffi/ansible-system.svg?style=social&label=Fork)](https://github.com/feffi/ansible-system) [![GitHub stars](https://img.shields.io/github/stars/feffi/ansible-system.svg?style=social&label=Star)](https://github.com/feffi/ansible-system) [![GitHub watchers](https://img.shields.io/github/watchers/feffi/ansible-system.svg?style=social&label=Watch)](https://github.com/feffi/ansible-system) [![Twitter Follow](https://img.shields.io/twitter/follow/feffi1.svg?style=social&label=Follow)](https://twitter.com/feffi1) [![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/feffi/ansible-system/blob/master/LICENSE)

## Requirements

- Ansible 2.7.1

### ansible.cfg

```yaml
hash_behaviour = merge
```

## Install

Just add the role to your ``requirements.yml`` file:

```yaml
- src: https://github.com/feffi/ansible-system.git
  name: ansible-system
```

## Role Defaults Variables

```yaml
ansible_system: {
  # The hostname to set
  hostname: "tardis"
}

```

Example:

```yaml
- hosts: all
  vars:
    ansible_system:
      # The hostname to set
      hostname: "tardis"
  roles:
    - { role: ansible-system }
```
