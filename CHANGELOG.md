# Docker Image Packaging for OpenJDK

## YYYYMMDD.Y.Z - TBC

### Major Changes

## 20220915.1.1 - 2022-09-15

### Major Changes

  - Support Ansible community package 6.4.0

## 20220824.1.1 - 2022-08-24

### Major Changes

  - Support Ansible community package 6.3.0

## 20220803.1.1 - 2022-08-03

### Major Changes

  - Support Ansible community package 6.2.0

## 20220714.1.1 - 2022-07-14

### Major Changes

  - Support Ansible community package 6.1.0
  - Remove Ubuntu 21.10 support

## 20220622.1.1 - 2022-06-22

### Major Changes

  - Support Ansible community package 6.0.0

## 20220608.1.1 - 2022-06-08

### Major Changes

  - Support Ansible community package 5.9.0

## 20220520.1.1 - 2022-05-20

### Major Changes

  - Support Ansible community package 5.8.0
  - Remove Fedora 34 support

## 20220427.1.1 - 2022-04-27

### Major Changes

  - Rename Ansible Role with FQCN
  - Support Ansible community package 5.7.0
  - Ubuntu 22.04 based
  - Support RHEL 9
  - Support CentOS 9 Stream
  - Support openSUSE Leap 15.4

## 20220407.1.2 - 2022-04-07

### Major Changes

  - Support Ansible community package 5.6.0
  - Support Fedora 36
  - Support Ubuntu 22.04
  - Support Ansible community package 5.5.0
  - Support Ansible community package 5.4.0

## 20220211.1.1 - 2022-02-11

### Major Changes

  - Remove Ubuntu 21.04 support
  - Skip package upgrade before running molecule

## 20211231.1.3 - 2021-12-31

### Major Changes

  - Support Fedora Rawhide
  - Support Debian Testing
  - Remove openSUSE Leap 15.2 support
  - Upgrade minimal Ansible community package support to 4.10

## 20211020.1.1 - 2021-10-20

### Major Changes

  - Install dependencies with package manager
  - Upgrade minimal Ansible community package support to 4.7.0

## 20210718.1.1 - 2021-07-18

### Major Changes

  - Upgrade minimal Ansible community package support to 4.2.0

## 20210602.1.1 - 2021-06-02

### Major Changes

  - Upgrade minimal Ansible support to 4.0.0

## 20210313.1.1 - 2021-03-13

### Major Changes

  - Bugfix [ansible-lint `namespace`](https://github.com/ansible-community/ansible-lint/pull/1451)
  - Bugfix [ansible-lint `no-handler`](https://github.com/ansible-community/ansible-lint/pull/1402)
  - Bugfix [ansible-lint `unnamed-task`](https://github.com/ansible-community/ansible-lint/pull/1413)
  - Change GIT tag as per Vagrant Box naming and versioning limitation

## 15.0.1-4alvistack4 - 2020-12-09

### Major Changes

  - Migrate from Travis CI to GitLab CI
  - Revamp with Packer

## 15.0.0-4alvistack2 - 2020-10-14

### Major Changes

  - Replace AdoptOpenJDK 14 with 15
  - Refine Molecule matrix

## 14.0.2-4alvistack2 - 2020-08-26

### Major Changes

  - Upgrade minimal Ansible Lint support to 4.3.2
  - Upgrade Travis CI test as Ubuntu Focal based
  - Upgrade minimal Ansible support to 2.10.0

## 14.0.1-4alvistack4 - 2020-06-10

### Major Changes

  - Revamp `create`, `side_effect`, `verify` and `destroy` logic
  - Replace `tini` with `catatonit`
  - Replace AdoptOpenJDK 13 with 14 for Ubuntu 20.04
  - Rename `post_tasks.yml` as `side_effect.yml`
  - Upgrade base image to Ubuntu 20.04

## 13.0.2-4alvistack4 - 2020-03-05

### Major Changes

  - Revamp with Molecule and `docker commit`
  - Consolidate molecule tests into `default` (noop)
  - Hotfix for systemd

## 13.0.1-3alvistack1 - 2020-01-15

### Major Changes

  - Replace `dumb-init` with `tini`, as like as `docker --init`
  - Include release specific vars and tasks

## 13.0.1-2alvistack1 - 2020-01-07

  - Ubuntu 18.04 based
  - Handle ENTRYPOINT with dumb-init
  - Self initialize with Ansible, by dogfooding with Ansible Playbook
