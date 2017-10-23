[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-virtualbox.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-virtualbox)

# Ansible Role: virtualbox

An Ansible role that installs virtualbox on Debian-like systems.

## Requirements

none

## Role Variables

```yaml

vbox_version: 5.1.30

vbox_build: 118389

# tar xf Oracle_VM_VirtualBox_Extension_Pack-5.1.30-118389.vbox-extpack
# openssl sha -sha256 ExtPack-license.txt
vbox_accept_license: b674970f720eb020ad18926a9268607089cc1703908696d24a04aa870f34c8e8

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
