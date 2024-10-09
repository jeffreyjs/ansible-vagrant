# Ansible Role: vagrant

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Install vagrant with Ansible

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml` and `vars/main.yml`):

Update the version of vagrant installed

```yaml
vagrant_update: false
```

Pin the version of vagrant to install, if omitted then it will query GitHub for the latest version. By default this is commented out.

```yaml
# vagrant_version: 2.4.1
```

## Dependencies

None.

## Example Playbook

The following is an example of how to use this role:

```yaml
- hosts: server
  vars_files:
    - vars/main.yml

  roles:
    - role: jeffreyjs.log2ram

  vars:
    vagrant_update: true
    vagrant_version: "2.4.1"
```

## License

MIT / BSD

## Author Information

[Jeffrey Swindel](https://github.com/jeffreyjs)
