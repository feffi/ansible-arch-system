# ansible-arch-system

Ansible role to maintain various general system settings.

[![Build Status](https://img.shields.io/travis/feffi/ansible-arch-system.svg)](https://travis-ci.org/feffi/ansible-arch-system) [![Github All Releases](https://img.shields.io/github/downloads/feffi/ansible-arch-system/total.svg)](https://github.com/feffi/ansible-arch-system) [![GitHub forks](https://img.shields.io/github/forks/feffi/ansible-arch-system.svg?style=social&label=Fork)](https://github.com/feffi/ansible-arch-system) [![GitHub stars](https://img.shields.io/github/stars/feffi/ansible-arch-system.svg?style=social&label=Star)](https://github.com/feffi/ansible-arch-system) [![GitHub watchers](https://img.shields.io/github/watchers/feffi/ansible-arch-system.svg?style=social&label=Watch)](https://github.com/feffi/ansible-arch-system) [![Twitter Follow](https://img.shields.io/twitter/follow/feffi1.svg?style=social&label=Follow)](https://twitter.com/feffi1) [![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/feffi/ansible-arch-system/blob/master/LICENSE)

## Requirements

- Ansible 2.7.1

### ansible.cfg

```yaml
hash_behaviour = merge
```

## Install

Just add the role to your ``requirements.yml`` file:

```yaml
- src: https://github.com/feffi/ansible-arch-system.git
  name: ansible-arch-system
```

## Role Defaults Variables

```yaml
ansible_arch_system: {
  # The hostname to set
  hostname: "tardis"
}

```

Example:

```yaml
- hosts: all
  vars:
    ansible_arch_system:
      # The hostname to set
      hostname: "tardis"
  roles:
    - { role: ansible-arch-system }
```
