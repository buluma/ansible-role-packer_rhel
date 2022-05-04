# [packer_rhel](#packer_rhel)

RedHat/CentOS configuration for Packer.

|GitHub|GitLab|Quality|Downloads|Version|Issues|Pull Requests|
|------|------|-------|---------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-packer_rhel/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-packer_rhel/actions)|[![gitlab](https://gitlab.com/buluma/ansible-role-packer_rhel/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-packer_rhel)|[![quality](https://img.shields.io/ansible/quality/)](https://galaxy.ansible.com/buluma/packer_rhel)|[![downloads](https://img.shields.io/ansible/role/d/)](https://galaxy.ansible.com/buluma/packer_rhel)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-packer_rhel.svg)](https://github.com/buluma/ansible-role-packer_rhel/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-packer_rhel.svg)](https://github.com/buluma/ansible-role-packer_rhel/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-packer_rhel.svg)](https://github.com/buluma/ansible-role-packer_rhel/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: Converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.packer_rhel
```

The machine needs to be prepared. In CI this is done using `molecule/default/prepare.yml`:
```yaml
---
- name: Prepare
  hosts: all
  gather_facts: no
  become: yes

  roles:
    - role: buluma.bootstrap
```


## [Role Variables](#role-variables)

The default values for the variables are set in `defaults/main.yml`:
```yaml
---
packer_rhel_libselinux_package: libselinux-python
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-packer_rhel/blob/main/requirements.txt).

## [Status of used roles](#status-of-requirements)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | GitLab |
|-------------|--------|--------|
|[buluma.bootstrap](https://galaxy.ansible.com/buluma/bootstrap)|[![Build Status GitHub](https://github.com/buluma/ansible-role-bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-bootstrap/actions)|[![Build Status GitLab ](https://gitlab.com/buluma/ansible-role-bootstrap/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-bootstrap)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-packer_rhel/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|el|all|

The minimum version of Ansible required is 2.12, tests have been done to:

- The previous version.
- The current version.
- The development version.



If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-packer_rhel/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-packer_rhel/blob/master/CHANGELOG.md)

## [License](#license)

license (Apache-2.0)

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
