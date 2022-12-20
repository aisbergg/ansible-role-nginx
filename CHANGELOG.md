# Changelog

All notable changes to this project will be documented in this file.

- [1.4.0 (2022-12-20)](#140-2022-12-20)
- [1.3.0 (2022-03-31)](#130-2022-03-31)
- [1.2.0 (2022-01-28)](#120-2022-01-28)
- [1.1.0 (2021-10-11)](#110-2021-10-11)
- [1.0.1 (2021-10-11)](#101-2021-10-11)
- [1.0.0 (2021-10-10)](#100-2021-10-10)

---

<a name="1.4.0"></a>
## [1.4.0](https://github.com/aisbergg/ansible-role-nginx/compare/v1.3.0...v1.4.0) (2022-12-20)

### Bug Fixes

- correct user for Arch Linux systems
- remove pid option, it is hardcoded in the service file
- make compatible with Debian systems
- linting issues
- fix removal of unmanaged vhost files

### Chores

- update linting config and add tox.ini

### Docs

- **README.md:** update documentation

### Features

- allow for other custom configs


<a name="1.3.0"></a>
## [1.3.0](https://github.com/aisbergg/ansible-role-nginx/compare/v1.2.0...v1.3.0) (2022-03-31)

### Bug Fixes

- make sure that pending handlers are run
- use full path of config file in validation task

### CI Configuration

- add branch explicitly to make Ansible import action happy
- bump Ansible Galaxy action version

### Chores

- update templates
- don't use bump2version to include the CHANGELOG in the bump commit, it doesn't do a good job

### Code Refactoring

- make cerficate copy tasks nicer

### Features

- add option 'nginx_create_dummy_certificate', that allows to create a TLS cert for testing purposes
- add option 'nginx_version', that allows to install a specific package version


<a name="1.2.0"></a>
## [1.2.0](https://github.com/aisbergg/ansible-role-nginx/compare/v1.1.0...v1.2.0) (2022-01-28)

### CI Configuration

- fix automatic release and publish process

### Chores

- include changelog in bump commits
- update included vhost template

### Features

- validate configuration after all vhosts have been created and add option to opt-out of validation


<a name="1.1.0"></a>
## [1.1.0](https://github.com/aisbergg/ansible-role-nginx/compare/v1.0.1...v1.1.0) (2021-10-11)

### Bug Fixes

- pacman module name

### Chores

- update changelog
- **requirements.yml:** add role requirements


<a name="1.0.1"></a>
## [1.0.1](https://github.com/aisbergg/ansible-role-nginx/compare/v1.0.0...v1.0.1) (2021-10-11)

### Bug Fixes

- trailing whitespaces

### Chores

- update changelog
- exclude .chglog/ from linting
- add bump2version config
- **.pre-commit-config.yaml:** bump pre-commit hook versions
- **CHANGELOG.tpl.md:** update changelog template


<a name="1.0.0"></a>
## [1.0.0]() (2021-10-10)

Initial Release
