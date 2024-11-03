[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Copier](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/copier-org/copier/master/img/badge/badge-grayscale-inverted-border.json)](https://github.com/copier-org/copier)
[![Podman Badge](https://img.shields.io/badge/Podman-892CA0?logo=podman&logoColor=white)](https://podman.io/)
[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
![CI](https://github.com/ansible-selfhosted/selfhosted.services.homepage/actions/workflows/ci.yml/badge.svg)
[![Ansible](https://img.shields.io/badge/Ansible-Molecule-EE0000?style=plastic&logo=ansible&logoColor=white)](https://github.com/ansible/molecule)

![](https://github.com/ansible-selfhosted/selfhosted.homepage/actions/workflows/ci.yaml/badge.svg)

<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: [homepage](https://gethomepage.dev/)

A role to deploy Homepage using rootless Podman with systemd.

## Role Requirements

- none

*Refer to services collection for general requirements*

## Role Arguments

|Option|Description|Type|Required|Default|
|---|---|---|---|---|
|config_path|The default path for the config files.|str|False|/home/{{ ansible_user_id }}/.config/homepage|
|docker_integration|Enables Docker integration.|bool|False|False|
|published_port|The default port for the web server.|int|False|3000|


## Example Playbook

```
- hosts: all
  tasks:
    - name: Importing homepage role
      ansible.builtin.import_role:
        name: selfhosted.services.homepage
      vars:
```

## License

This project is licensed under the [MIT License](LICENSE)


⊂(▀¯▀⊂)

<!-- END_ANSIBLE_DOCS -->
