# [Ansible role packer_rhel](#packer_rhel)

RedHat/CentOS configuration for Packer.

|GitHub|GitLab|Downloads|Version|Issues|Pull Requests|
|------|------|-------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-packer_rhel/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-packer_rhel/actions/workflows/molecule.yml)|[![gitlab](https://gitlab.com/shadowwalker/ansible-role-packer_rhel/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-packer_rhel)|[![downloads](https://img.shields.io/ansible/role/d/4793)](https://galaxy.ansible.com/buluma/packer_rhel)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-packer_rhel.svg)](https://github.com/buluma/ansible-role-packer_rhel/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-packer_rhel.svg)](https://github.com/buluma/ansible-role-packer_rhel/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-packer_rhel.svg)](https://github.com/buluma/ansible-role-packer_rhel/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-packer_rhel/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
---
- name: Converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.packer_rhel
```

The machine needs to be prepared. In CI this is done using [`molecule/default/prepare.yml`](https://github.com/buluma/ansible-role-packer_rhel/blob/master/molecule/default/prepare.yml):

```yaml
---
- name: Prepare
  hosts: all
  gather_facts: no
  become: yes

  roles:
    - role: buluma.bootstrap
    - role: buluma.hostname
    - role: buluma.openssh
```

Also see a [full explanation and example](https://buluma.github.io/how-to-use-these-roles.html) on how to use these roles.

## [Role Variables](#role-variables)

The default values for the variables are set in [`defaults/main.yml`](https://github.com/buluma/ansible-role-packer_rhel/blob/master/defaults/main.yml):

```yaml
---
packer_rhel_libselinux_package: libselinux-python
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-packer_rhel/blob/master/requirements.txt).

## [State of used roles](#state-of-used-roles)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | GitLab |
|-------------|--------|--------|
|[buluma.bootstrap](https://galaxy.ansible.com/buluma/bootstrap)|[![Build Status GitHub](https://github.com/buluma/ansible-role-bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-bootstrap/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-bootstrap/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-bootstrap)|
|[buluma.hostname](https://galaxy.ansible.com/buluma/hostname)|[![Build Status GitHub](https://github.com/buluma/ansible-role-hostname/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-hostname/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-hostname/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-hostname)|
|[buluma.openssh](https://galaxy.ansible.com/buluma/openssh)|[![Build Status GitHub](https://github.com/buluma/ansible-role-openssh/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-openssh/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-openssh/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-openssh)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-packer_rhel/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|[EL](https://hub.docker.com/repository/docker/buluma/enterpriselinux/general)|8|

The minimum version of Ansible required is 2.12, tests have been done to:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-packer_rhel/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-packer_rhel/blob/master/CHANGELOG.md)

## [License](#license)

[license (Apache-2.0)](https://github.com/buluma/ansible-role-packer_rhel/blob/master/LICENSE).

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)

Please consider [sponsoring me](https://github.com/sponsors/buluma).

### [Special Thanks](#special-thanks)

Template inspired by [Robert de Bock](https://github.com/robertdebock)
