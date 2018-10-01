[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-virtualbox.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-virtualbox)

# lifeofguenter.virtualbox

An Ansible role that installs virtualbox on Debian-like systems.

## Versions

Use tag/version pinning to achieve your goal:

| Version | VirtualBox | Latest | Status     |
| ------- | ---------- | ------ | ---------- |
| 0.2.x   | 5.2        | 5.2.18 | active     |
| 0.1.x   | 5.1        | 5.1.38 | deprecated |

## Requirements

none

## Role Variables

```yaml

vbox_version: 5.2.18

# tar xf Oracle_VM_VirtualBox_Extension_Pack-5.2.18.vbox-extpack
# openssl sha -sha256 ExtPack-license.txt
vbox_accept_license: 56be48f923303c8cababb0bb4c478284b688ed23f16d775d729b89a2e8e5f9eb
```

## Dependencies

none

## Example Playbook

```yaml

- hosts: virtualbox-hosts
  roles:
    - { role: lifeofguenter.virtualbox }
```

## License

Licensed under the MIT License. See the [LICENSE file](LICENSE) for details.

## Author Information

[Gunter Grodotzki](https://lifeofguenter.de)
