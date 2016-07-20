# FQDN

[![Ansible Galaxy][galaxy_image]][galaxy_link]
[![Build Status][travis_image]][travis_link]
[![Latest tag][tag_image]][tag_url]
[![Gitter chat][gitter_image]][gitter_url]

A role for managing the fqdn/hostname.

## Requirements

- Hosts should be bootstrapped for ansible usage (have python,...)
- Root privileges, eg `become: yes`

## Role Variables

| Variable | Description | Default value |
|----------|-------------|---------------|
| `fqdn_full` | Fully qualified domain name | `inventory_hostname` |
| `fqdn_short` | Short hostname | `inventory_hostname_short` |

## Dependencies

None.

## Example Playbook

```yaml
---
- hosts: test
  roles:
  - { role: GROG.fqdn, become: yes }
```

## Contributing
All assistance, changes or ideas [welcome][issues]!

## Author
By [G. Roggemans][groggemans]

## License
MIT

[galaxy_image]:         https://img.shields.io/badge/galaxy-GROG.fqdn-660198.svg?style=flat
[galaxy_link]:          https://galaxy.ansible.com/GROG/fqdn
[travis_image]:         https://travis-ci.org/GROG/ansible-role-fqdn.svg?branch=master
[travis_link]:          https://travis-ci.org/GROG/ansible-role-fqdn
[tag_image]:            https://img.shields.io/github/tag/GROG/ansible-role-fqdn.svg
[tag_url]:              https://github.com/GROG/ansible-role-fqdn/tags
[gitter_image]:         https://badges.gitter.im/GROG/chat.svg
[gitter_url]:           https://gitter.im/GROG/chat

[issues]:               https://github.com/GROG/ansible-role-fqdn/issues
[groggemans]:           https://github.com/groggemans
