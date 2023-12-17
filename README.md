# [Ansible role brightbox_ruby](#brightbox_ruby)

Install Brightbox ruby packages on your systems.

|GitHub|GitLab|Downloads|Version|Issues|Pull Requests|
|------|------|-------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-brightbox_ruby/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-brightbox_ruby/actions/workflows/molecule.yml)|[![gitlab](https://gitlab.com/shadowwalker/ansible-role-brightbox_ruby/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-brightbox_ruby)|[![downloads](https://img.shields.io/ansible/role/d/)](https://galaxy.ansible.com/buluma/brightbox_ruby)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-brightbox_ruby.svg)](https://github.com/buluma/ansible-role-brightbox_ruby/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-brightbox_ruby.svg)](https://github.com/buluma/ansible-role-brightbox_ruby/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-brightbox_ruby.svg)](https://github.com/buluma/ansible-role-brightbox_ruby/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-brightbox_ruby/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
---
- name: converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.brightbox_ruby
      brightbox_ruby_psp_pkg_state: latest
```

Also see a [full explanation and example](https://buluma.github.io/how-to-use-these-roles.html) on how to use these roles.

## [Role Variables](#role-variables)

The default values for the variables are set in [`defaults/main.yml`](https://github.com/buluma/ansible-role-brightbox_ruby/blob/master/defaults/main.yml):

```yaml
---
# defaults file for brightbox_ruby
brightbox_ruby_psp_pkg_version:
brightbox_ruby_psp_pkg_state: installed
brightbox_ruby_packages:
  - ruby2.4
  - ruby2.4-dev
brightbox_ruby_gem_user_install: no
brightbox_ruby_gems:
  - rake
  - bundler
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-brightbox_ruby/blob/master/requirements.txt).


## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-brightbox_ruby/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|[Debian](https://hub.docker.com/repository/docker/buluma/debian/general)|all|
|[Ubuntu](https://hub.docker.com/repository/docker/buluma/ubuntu/general)|all|

The minimum version of Ansible required is 2.12, tests have been done to:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-brightbox_ruby/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-brightbox_ruby/blob/master/CHANGELOG.md)

## [License](#license)

[Apache-2.0](https://github.com/buluma/ansible-role-brightbox_ruby/blob/master/LICENSE).

## [Author Information](#author-information)

[buluma](https://buluma.github.io/)

Please consider [sponsoring me](https://github.com/sponsors/buluma).

### [Special Thanks](#special-thanks)

Template inspired by [Robert de Bock](https://github.com/robertdebock)
