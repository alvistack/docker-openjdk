# Docker Image Packaging for OpenJDK

## 13.0.2-XalvistackY - TBC

### Major Changes

## 13.0.2-4alvistack7 - 2020-04-11

### Major Changes

  - Provision with systemd support

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
